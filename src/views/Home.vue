<template>
  <div class="home">
    <v-container>
   <h2 class="text-h5 text-center mb-3 mt-5">Brasileirão Série A</h2>
    <v-img class="ini-img mb-4" src="https://diariodonordeste.verdesmares.com.br/image/contentid/policy:1.2974821:1596806515/Serie-A.png"/>
    <p> A Série A do Campeonato Brasileiro de Futebol de 2020, oficialmente Brasileirão Assaí – Série A 2020 por motivos de patrocínio, é a 64.ª edição da principal divisão do futebol brasileiro. A disputa tem o mesmo regulamento dos anos anteriores, quando foi implementado o sistema de pontos corridos.</p>
    <p class="pb-4 text-h6 text-center mb-5"><strong >Se voce não curtir seu time vai cair!! </strong>{{cont}}</p>
    </v-container>
    <v-btn
      class="mx-2"
      fab
      dark
      small
      color="teal darken-2"
      @click="like"
    >
      <v-icon dark>
        mdi-thumb-up
      </v-icon>
    </v-btn>
  </div>
</template>

<script>

export default {
  name: 'Home',
  components: {
  },
  data(){
    return{
      cont: 0
    }
  },
  methods:{
    like(){
      this.cont ++
    }
  }
}
</script>
<style scoped>
    .ini-img {
        border-radius: 8px;
    }
</style>
