<script setup>
import { ref } from 'vue';
import Cabecalho from './components/cabecalho.vue';
import Post from './components/post.vue';
import Login from './components/login.vue'; 


import rimuruImage4 from './assets/logoG1.png';

const nomeUsuario = ref(''); // Estado para armazenar o nome do usuário

const handleLogin = (usuario) => {
  nomeUsuario.value = usuario; // Atualiza o nome do usuário
};
</script>

<template>
  <div>
    <Cabecalho 
      :img_cabec="rimuruImage4" 
      :titulo="nomeUsuario || 'Rimuru_'" /> 
    
    <Login v-if="!nomeUsuario" @login="handleLogin" /> 
    
    <router-view v-if="nomeUsuario" /> 
  </div>
  <!--<div>
    <Cabecalho 
      :img_cabec="rimuruImage4" 
      titulo="Rimuru_" />
    
    <router-view/>
    
 
    <Post 
      :img_post="rimuruImage1"
      tit_post="Introdução" 
      mes_post="Rimuru Tempest, o protagonista de Tensei Shitara Slime Datta Ken, alcançou um feito impressionante ao derrotar 20.000 soldados durante sua transformação em Lorde Demônio. Este evento não apenas destacou sua força extraordinária, mas também solidificou sua posição como um dos seres mais poderosos do mundo, capaz de aniquilar um exército inteiro com uma combinação de habilidades mágicas e estratégias astutas." 
      autor_post="Wesley"
    />
    
    <Post 
      :img_post="rimuruImage2"
      tit_post="Reflexão" 
      mes_post="A ascensão de Rimuru ao título de Lorde Demônio não foi apenas uma questão de poder, mas também de responsabilidade. Ele usou suas novas habilidades para proteger seu povo e estabelecer uma era de paz, mostrando que a verdadeira força reside na capacidade de proteger aqueles que amamos." 
      autor_post="Wesley"
    />
    
    <Post 
      :img_post="rimuruImage3"
      tit_post="Finalização" 
      mes_post="Com isso, deixo uma reflexão: em um mundo repleto de conflitos, que possamos encontrar inspiração na jornada de Rimuru e buscar sempre a paz, mesmo diante das adversidades. Até a próxima!" 
      autor_post="Wesley"
    />
    
    <Login 
      :imgLogo="rimuruImage4"
    />
  </div>-->
</template>

<style scoped>
header {
  line-height: 1.5;
  background-color: rgb(0, 0, 0);
  width: 710px;
  height: 670px;
}
h1 {
  font-size: 70px;
  font-weight: bolder;
}
h2 {
  font-weight: bolder;
}
</style>
