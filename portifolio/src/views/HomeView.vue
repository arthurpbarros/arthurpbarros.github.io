<script setup lang="ts">
import TheWelcome from '../components/TheWelcome.vue'
import Django from '../assets/Django.png'
import Next from '../assets/Next.js.png'
import React from '../assets/React.png'
import VueJS from '../assets/Vue.js.png'
import unsplash from '../assets/unsplash.jpg'
// import Image from '../../public/img/perfil1.png'


import { ref } from 'vue'
const framework = ref('')
const atual = ref(0);

function choiceFramework(framework_str: string){
  framework.value = framework_str;
}
</script>

<template>
  <main>
    <section id="inicio" class="">
      <div class="w-full min-h-screen">
        <div
          class="w-full lg:mx-auto gap-2 flex flex-col lg:flex-row justify-center bg-linear-to-tl from-black from-70% to-gray-900 itens-center min-h-screen">
          <div class="lg:w-2/5 w-4/5 flex flex-col justify-center itens-center mx-auto rounded-full">
            <h1
              class="leading-18 text-white text-5xl lg:text-6xl pt-10 rounded-tr-4xl rounded-bl-4xl transition-all animate-pulse delay-1000 p-6">
              Sou
              <span class="text-green-600 font-bold">Arthur</span>, desenvolvedor fullstack
              focado em
              desenvolver <span class=" bg-green-600 px-3 rounded-2xl"> aplicações web </span>
            </h1>
          </div>
          <div class="w-full lg:w-1/2 min-h-screen flex flex-col justify-center itens-start">
            <div class="w-full mx-auto bg-cover fundo min-h-screen bg-blend-darken bg-green-600 rounded-tl-3xl"></div>
          </div>
        </div>
      </div>
    </section>

    <section id="inicio" class="py-8">
      <h1 class="leading-18 text-green-600 text-center text-5xl lg:text-6xl rounded-tr-4xl rounded-bl-4xl p-6">
        Tecnologias
      </h1>
      <div class="flex flex-row w-3/4 justify-center mx-auto">
        <div class="lg:block hidden w-1/4 min-h-full">
          <div class="w-full text-white bg-linear-0 to-100% from-black to-gray-900 min-h-full flex flex-col justify-center gap-5 p-8 rounded-xl" v-show="framework === 'vue'">
            <h1 class="uppercase text-green-500 text-xl">Vue</h1>
            <p class="font-light"> Vue é uma biblioteca javascript para criação de interfaces baseadas em componentes reutilizáveis </p>
          </div>
          <div class="w-full text-white bg-linear-0 to-100% from-black to-gray-900 min-h-full flex flex-col justify-center gap-5 p-8 rounded-xl" v-show="framework === 'django'">
            <h1 class="uppercase text-green-500 text-xl">Django</h1>
            <p> é um framework python para desenvolvimento rápido </p>
          </div>
        </div>
        <div class="w-1/4 mx-auto">
          <div class="grid grid-cols-2 gap-x-30 gap-y-15 w-full mx-auto">
            <div class="bg-django min-w-20 min-h-20 bg-cover rounded-xl hover:scale-125 grayscale hover:grayscale-0" @mouseenter="choiceFramework('django')"></div>
            <div class="bg-vue min-w-20 min-h-20 bg-cover rounded-xl hover:scale-125 grayscale hover:grayscale-0" @mouseenter="choiceFramework('vue')"></div>
            <div class="bg-react min-w-20 min-h-20 bg-cover rounded-xl hover:scale-125 grayscale hover:grayscale-0" @mouseenter="choiceFramework('react')"></div>
            <div class="bg-next min-w-20 min-h-20 bg-cover rounded-xl hover:scale-125 grayscale hover:grayscale-0" @mouseenter="choiceFramework('next')"></div>
          </div>
        </div>
        <div class="lg:block hidden w-1/4 min-h-full">
          <div class="w-full text-white bg-linear-0 to-100% from-black to-gray-900 min-h-full flex flex-col justify-center gap-5 p-8 rounded-xl" v-show="framework === 'react'">
            <h1 class="uppercase text-green-500 text-xl">React</h1>
            <p> React é uma biblioteca javascript para criação de interfaces baseadas em componentes reutilizáveis </p>
          </div>
          <div class="w-full text-white bg-linear-0 to-100% from-black to-gray-900 min-h-full flex flex-col justify-center gap-5 p-8 rounded-xl" v-show="framework === 'next'">
            <h1 class="uppercase text-green-500 text-xl">Next</h1>
            <p> é um framework javascript para criação de aplicações fullstack, utiliza o React </p>
          </div>
        </div>
      </div>
    </section>

    <section id="sobre">
      <div class="p-8 flex flex-col lg:flex-row bg-linear-to-b lg:bg-linear-to-r from-0% to-100% from-black to-green-500">
        <img :src=unsplash alt="" class="lg:w-1/2 w-full rounded-xl">
        <div class="relative top-0 left-0"></div>
        <div class="flex flex-col gap-6 justify-center lg:w-1/2 w-full">
          <p class="p-8 text-white text-3xl"> Sou desenvolvedor fullstack, atualmente focado em front-end, estusiasta por
            tecnologia
            e que gosta de criar interfaces responsivas e agradáveis ao usuário
          <div class="flex flex-col gap-4 ml-4 text-2xl">
            <div class="text-white bg-black p-4 rounded-full hover:text-green-500">
              CURSO TÉCNICO INTEGRADO EM INFORMÁTICA
            </div>
            <div class="text-white bg-black p-4 rounded-full hover:text-green-500">
              GRADUAÇÃO EM ANÁLISE DE SISTEMAS
            </div>
          </div>
          </p>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <p>&copy; 2024 Todos os direitos reservados.</p>
  </footer>
</template>
