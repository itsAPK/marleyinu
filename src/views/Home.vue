<template>
<NavBar/>
  <section id='home'>
    <div  class="flex items-center justify-center m-5" >
           <img alt="Marley Inu" src="../assets/logo.png" class="lg:w-1/4 w-fit animate__animated animate__fadeInDown animate__fast">
    </div>
    <div  class="flex items-center justify-center m-1" >
        <h1 class="inline-flex text-6xl sm:text-5xl text-amber-400  font-extrabold font-rubik animate__animated animate__fadeInLeft animate__fast uppercase ">Marley&nbsp; </h1>
        <h1 class="inline-flex text-6xl sm:text-5xl text-amber-400  font-bold font-rubik animate__animated animate__fadeInRight animate__fast uppercase ">Inu</h1>
    </div>
    <h2 class="text-yellow-600 font-black animate__animated  animate__fadeInUp animate__fast uppercase font-electrolize ">
      A decentralized deflationary memetoken
    </h2>
   <div class=" items-center justify-between px-10 py-5 mt-5 lg:px-32 lg:py-10 columns-xl">
     <p class="text-justify text-amber-400 lg:text-2xl font-lexend  uppercase mt-5 lg:mt-16 ">Introduction</p>
    <div class="inline-flex">
     <p class=" text-neutral-100 lg:text-justify text-sm  font-raleway font-black uppercase mt-4  ">
    Marley Inu $minu is built by a strong team of crypto experts. We aim to build a sustainable, long term memetoken bringing innovative ideas in the  cryptospace. In addition, we aim to build a complete ecosystem with our utilities and this can be accomplished by a strong and connected community.
    </p>
    </div>
     <div class="lg:flex items-center justify-between py-10 m-2">
    <div class="inline-flex">
          <button class="h-10 px-6 mr-8 text-yellow-500 text-xl font-lexend400 transition-colors duration-150 border border-yellow-500 rounded-sm focus:shadow-outline hover:bg-yellow-500 hover:text-black"><a href="https://www.dextools.io/app/bsc/pair-explorer/0xAD3d2c978eA1a24a3D895001e4E8db3e04A07401">CHART</a></button>
            <button class="h-10 px-8 text-yellow-500  text-xl font-lexend400 transition-colors duration-150 border border-yellow-500 rounded-sm focus:shadow-outline hover:bg-yellow-500 hover:text-black"><a href="https://pancakeswap.finance/swap?outputCurrency=0x1FAFBFb8d51c8Dbb66B5b59DaeCcE14b82F5b0d9">BUY</a></button>
    </div>
  </div></div>
  </section>
  <Tokenomics/>
  <Roadmap/>
  <Footer/>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
// import HelloWorld from '@/components/HelloWorld.vue' // @ is an alias to /src

import NavBar from '@/components/NavBar.vue'
import Tokenomics from './Tokenomics.vue'
import Roadmap from './Roadmap.vue'
import Footer from './Footer.vue'
export default defineComponent({
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Home',
  components: {
    NavBar,
    Tokenomics,
    Roadmap,
    Footer
  }
})
</script>
