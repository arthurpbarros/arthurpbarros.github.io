<script setup lang="ts">
import TheWelcome from '../components/TheWelcome.vue'
import Django from '../assets/Django.png'
import Next from '../assets/Next.js.png'
import React from '../assets/React.png'
import VueJS from '../assets/Vue.js.png'
import unsplash from '../assets/unsplash.jpg'
// import Image from '../../public/img/perfil1.png'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faHtml5, faCss3, faPython, faDocker, faJs } from '@fortawesome/free-brands-svg-icons'
import Daiane from '@/assets/projects/daiane.png'

import { ref } from 'vue'
const framework = ref('')
const atual = ref(0);

function choiceFramework(framework_str: string) {
  framework.value = framework_str;
}
</script>

<template>
  <main>
    <section id="inicio" class="">
      <div class="w-full min-h-screen">
        <div
          class="w-full lg:mx-auto gap-2 flex flex-col lg:flex-row justify-center bg-linear-to-tl from-indigo-900 from-70% to-gray-600 itens-center min-h-screen">
          <div class="lg:w-2/5 w-4/5 flex flex-col justify-center itens-center mx-auto rounded-full">
            <h1
              class="leading-16 sm:leading-18 text-white text-5xl lg:text-6xl pt-10 rounded-tr-4xl rounded-bl-4xl transition-all animate-pulse delay-1000 p-6">
              Sou
              <span class="text-lime-500 font-bold">Arthur</span>, desenvolvedor fullstack
              focado em
              desenvolver <span class=" bg-lime-500 px-3 rounded-2xl text-indigo-900"> aplicações web </span>
            </h1>
          </div>
          <div class="w-full lg:w-1/2 min-h-screen flex flex-col justify-center itens-start">
            <div class="w-full mx-auto bg-cover fundo min-h-screen bg-blend-darken bg-lime-500 rounded-tl-3xl"></div>
          </div>
        </div>
      </div>
    </section>

    <section id="inicio" class="py-8">
      <h1 class="leading-18 text-indigo-900 text-center text-5xl lg:text-6xl rounded-tr-4xl rounded-bl-4xl p-6">
        Tecnologias
      </h1>
      <div class="flex flex-row w-3/4 justify-center mx-auto">
        <div class="flex flex-row gap-5 mx-auto items-center">
          <div
            class="bg-django min-w-20 min-h-20 bg-center bg-contain rounded-xl hover:scale-125 grayscale hover:grayscale-0"
            @mouseenter="choiceFramework('django')"></div>
          <div
            class="bg-vue min-w-20 min-h-20 bg-center bg-contain rounded-xl hover:scale-125 grayscale hover:grayscale-0"
            @mouseenter="choiceFramework('vue')"></div>
          <div
            class="bg-react min-w-20 min-h-20 bg-center bg-contain rounded-xl hover:scale-125 grayscale hover:grayscale-0"
            @mouseenter="choiceFramework('react')"></div>
          <div
            class="bg-next min-w-20 min-h-20 bg-center bg-contain rounded-xl hover:scale-125 grayscale hover:grayscale-0"
            @mouseenter="choiceFramework('next')"></div>
        </div>
      </div>
    </section>

    <section id="sobre" class="w-5/6 rounded-xl mx-auto fundo_code bg-cover bg-left shadow-xl shadow-gray-500">
      <div
        class="p-8 flex flex-col lg:flex-row bg-linear-to-r from-indigo-900 via-indigo-700/90 via-70% lg:to-indigo-700/40 to-indigo-700/80 bg-cover rounded-xl">
        <!-- <img :src=unsplash alt="" class="lg:w-1/2 w-full rounded-xl"> -->
        <div class="relative top-0 left-0"></div>
        <div class="flex flex-col gap-6 justify-center lg:w-1/2 w-full">
          <p class="p-8 text-white text-3xl"> Sou desenvolvedor fullstack, atualmente focado em front-end,
            estusiasta
            por
            tecnologia
            e que gosta de criar interfaces responsivas e agradáveis ao usuário
          <div class="flex flex-col gap-4 ml-4 text-xl font-serif">
            <div class="p-4 rounded-xl hover:scale-105 font-bold bg-lime-500 text-indigo-900">
              Curso Técnico Integrado em Informática
            </div>
            <div class="p-4 rounded-xl hover:scale-105 font-bold bg-lime-500 text-indigo-900">
              Graduação em Análise de Sistemas
            </div>
          </div>
          </p>
        </div>
      </div>
    </section>


    <section id="sobre" class="w-full mx-auto mt-20 py-15 bg-indigo-900">
      <div class="p-8">
        <h2 class="leading-18 text-white text-center text-5xl lg:text-6xl rounded-tr-4xl rounded-bl-4xl pb-6">
          Habilidades
        </h2>
        <div class="w-3/4 mx-auto flex flex-row gap-5 font-serif text-white">
          <div class="w-1/2 flex flex-col gap-2">
            <div>
              <div class="flex flex-row gap-5 border border-white p-4 rounded-xl">
                <FontAwesomeIcon :icon="faHtml5" class="fa-4x text-lime-500" />
                <div class="w-full flex flex-col justify-center itens-start">
                  <h3>HTML</h3>
                  <div
                    class="bg-lime-500 w-full h-6 rounded-r-xl text-center text-xs font-bold text-indigo-900 flex flex-col justify-center shadow-xl">
                    100%</div>
                </div>
              </div>
            </div>
            <div>
              <div class="flex flex-row gap-5 border border-white p-4 rounded-xl">
                <FontAwesomeIcon :icon="faCss3" class="fa-4x" />
                <div class="w-full flex flex-col justify-center itens-start">
                  <h3>CSS</h3>
                  <div
                    class="bg-white w-3/5 h-6 rounded-r-xl text-center text-xs font-bold text-indigo-900 flex flex-col justify-center shadow-xl">
                    100%</div>
                </div>
              </div>
            </div>
            <div>
              <div class="flex flex-row gap-5 border border-white p-4 rounded-xl">
                <FontAwesomeIcon :icon="faJs" class="fa-4x text-lime-500" />
                <div class="w-full flex flex-col justify-center itens-start">
                  <h3>JS</h3>
                  <div
                    class="bg-lime-500 w-1/2 h-6 rounded-r-xl text-center text-xs font-bold text-indigo-900 flex flex-col justify-center shadow-xl">
                    100%</div>
                </div>
              </div>
            </div>
          </div>
          <div class="w-1/2 flex flex-col gap-2">
            <div>
              <div class="flex flex-row gap-5 border border-white p-4 rounded-xl">
                <FontAwesomeIcon :icon="faPython" class="fa-4x" />
                <div class="w-full flex flex-col justify-center itens-start">
                  <h3>Python</h3>
                  <div
                    class="bg-lime-500 w-full h-6 rounded-r-xl text-center text-xs font-bold text-indigo-900 flex flex-col justify-center shadow-xl">
                    100%</div>
                </div>
              </div>
            </div>
            <div>
              <div class="flex flex-row gap-5 border border-white p-4 rounded-xl">
                <FontAwesomeIcon :icon="faDocker" class="fa-4x text-lime-500" />
                <div class="w-full flex flex-col justify-center itens-start">
                  <h3>Docker</h3>
                  <div
                    class="bg-white w-4/5 h-6 rounded-r-xl text-center text-xs font-bold text-indigo-900 flex flex-col justify-center shadow-xl">
                    100%</div>
                </div>
              </div>
            </div>
            <div>
              <div class="flex flex-row gap-5 border border-white p-4 rounded-xl">
                <FontAwesomeIcon :icon="faHtml5" class="fa-4x" />
                <div class="w-full flex flex-col justify-center itens-start">
                  <h3>JS</h3>
                  <div
                    class="bg-lime-500 w-1/2 h-6 rounded-r-xl text-center text-xs font-bold text-indigo-900 flex flex-col justify-center shadow-xl">
                    100%</div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>

  <section id="sobre" class="w-full mx-auto py-15 bg-lime-500">
    <div class="p-8">
      <h2 class="leading-18 text-indigo-900 text-center text-5xl lg:text-6xl rounded-tr-4xl rounded-bl-4xl pb-6">
        Projetos
      </h2>
      <div class="w-5/6 mx-auto flex flex-col sm:flex-row gap-5 text-white">
        <div class="bg-indigo-900 flex flex-col justify-center rounded-t-xl shadow-indigo-900 shadow-2xl">
          <img :src=Daiane alt="" class="mx-auto rounded-t-xl">
          <div class= "bg-indigo-900 flex flex-col gap-5 justify-center p-5">
            <h3 class="text-white text-xl sm:text-lg xl:text-xl text-left border-b">Landing Page Fisioterapia</h3>
            <p class="font-serif">Sistema para atendimentos da fisioterapeuta Daiane Carla</p>
          </div>
        </div>
        <div class="bg-indigo-900 flex flex-col justify-center rounded-t-xl shadow-indigo-900 shadow-2xl">
          <img :src=Daiane alt="" class="mx-auto rounded-t-xl">
          <div class= "bg-indigo-900 flex flex-col gap-5 justify-center p-5">
            <h3 class="text-white text-xl sm:text-lg xl:text-xl text-left border-b">Landing Page Fisioterapia</h3>
            <p class="font-serif">Sistema para atendimentos da fisioterapeuta Daiane Carla</p>
          </div>
        </div>
        <div class="bg-indigo-900 flex flex-col justify-center rounded-t-xl shadow-indigo-900 shadow-2xl">
          <img :src=Daiane alt="" class="mx-auto rounded-t-xl">
          <div class= "bg-indigo-900 flex flex-col gap-5 justify-center p-5">
            <h3 class="text-white text-xl sm:text-lg xl:text-xl text-left border-b">Landing Page Fisioterapia</h3>
            <p class="font-serif">Sistema para atendimentos da fisioterapeuta Daiane Carla</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <footer>
    <p>&copy; 2024 Todos os direitos reservados.</p>
  </footer>
</template>
