<script setup>
// Props comentados
// const props = defineProps({
//   tit_post: {
//     type: String,
//     required: false
//   },
//   mes_post: {
//     type: String,
//     required: false
//   },
//   autor_post: {
//     type: String,
//     required: false
//   },
//   img_post: {
//     type: String,
//     required: false
//   }
// });
</script>
<template>
  <div class="post">
    <img src="@/assets/timao.jpg" alt="Imagem do Post" width="100%" height="auto" />
    <h2>Corinthians</h2>
    <p>Primeiro Campeão mundial Fifa do brasil. 30x campeão paulista, 7x campeão do campeonato brasileiro, 3x campeão da copa do brasil, 1x campeão continental e 2x campeão Mundial.</p>
    <p class="autor">Matheus</p>
  </div>

  <div class="post">
    <img src="@/assets/bortoleto.jpg" alt="Imagem do Post" width="100%" height="auto" />
    <h2>Brasil na F1  </h2>
    <p>O Brasil finalmente tem um piloto titular na Formula 1! Depois de sete anos Gabriel Bortoleto representará a Bandeira brasileira na maior competição automobilistica do mundo.</p>
    <p class="autor">Matheus</p>
  </div>

  <div class="post">
    <img src="@/assets/apostas.jpg" alt="Imagem do Post" width="100%" height="auto" />
    <h2>Mais um caso de manipulação</h2>
    <p>Bruno henrique, atacante do flamengo é o acusado da vez! Jogador está sendo investigado por supostamente manipular um cartão vermelho na partida contra o Santos pelo brasileirão, a fim de ajudar familiares e amigos.</p>
    <p class="autor">Matheus</p>
  </div>
</template>



<style scoped>
.post {
  background-color: gainsboro;
  margin-bottom: 20px;
  padding: 20px;
  border-radius: 5px; /* Adiciona bordas arredondadas */
}

.autor {
  color: black;
  text-align: right;
  margin: 0;
  font-size: 0.8em;
}
</style>
