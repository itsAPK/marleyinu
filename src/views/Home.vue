<template>
<NavBar/>
  <section id='home'>
    <div  class="flex items-center justify-center m-16" >
           <img alt="Marley Inu" src="../assets/logo.png" class=" animate__animated animate__fadeInDown animate__fast">
    </div>
    <div  class="flex items-center justify-center m-7" >
        <h1 class="inline-flex text-6xl text-amber-400  font-extrabold font-rubik animate__animated animate__fadeInLeft animate__fast uppercase ">Marley&nbsp; </h1>
        <h1 class="inline-flex text-6xl text-amber-400  font-bold font-rubik animate__animated animate__fadeInRight animate__fast uppercase ">Inu</h1>
    </div>
    <h2 class="text-yellow-600 font-black animate__animated  animate__fadeInUp animate__fast uppercase font-electrolize ">
      A decentralized deflationary memetoken
    </h2>
   <div class=" items-center justify-between px-10 py-5 mt-5 lg:px-32 lg:py-10 columns-xl">
     <p class="text-justify text-amber-400 lg:text-2xl font-lexend  uppercase mt-5 lg:mt-16 ">Introduction</p>
     <div class="lg:columns-2">
    <div class="inline-flex">
     <p class=" text-neutral-100 text-md font-raleway font-black uppercase mt-4 " >
      Marley Inu $minu is built by a strong team of crypto experts. We aim to build a sustainable, long term memetoken bringing innovative ideas in the  cryptospace. In addition, we aim to build a complete ecosystem with our utilities and this can be accomplished by a strong and connected community.
    </p>
    </div>
    <div class="inline-flex">
     <img alt="Marley Inu" src="../assets/dollar.png" width="250" class=" animate__animated animate__fadeInRight animate__fast mt-2 lg:mt-0 ">
    </div>
  </div></div>
  </section>
  <Tokenomics/>
  <Roadmap/>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
// import HelloWorld from '@/components/HelloWorld.vue' // @ is an alias to /src

import NavBar from '@/components/NavBar.vue'
import Tokenomics from './Tokenomics.vue'
import Roadmap from './Roadmap.vue'
export default defineComponent({
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Home',
  components: {
    NavBar,
    Tokenomics,
    Roadmap
  }
})
</script>
