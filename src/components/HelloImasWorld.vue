<template>
  <div>
    <b-button v-on:click="getidol">GET!!!</b-button>
    <hr>
    {{hei}}
  </div>
</template>

<script>
import idolheight from 'raw-loader!../api/query/heightorder.sparql'
import axios from 'axios';

export default {
  name: 'HelloImasWorld',
  data: () => ({
    hei: ''
  }),
  methods: {
    getidol() {
      console.log('開始1')
      const url = 'https://sparql.crssnky.xyz/spql/imas/query';
        console.log('開始2')
        axios.get(url, {
          params: {
            query: idolheight
          }
        }).then((e) => {
          this.hei = e;
        })
    }
  }
}
</script>

<style scoped>
</style>
