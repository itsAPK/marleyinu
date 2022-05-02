/* eslint-disable vue/multi-word-component-names */
// eslint-disable-next-line vue/multi-word-component-names
<template>
  <section id="tokenomics" style="background-color: #de9f00">
  <div class="lg:columns-2  container  items-center justify-between lg:p-10">
    <div class="inline-flex  col-span-3 flex-col m-1">
      <h1 class="text-6xl font-barlow uppercase font-extrabold text-gray-800 pt-16">Tokenomics</h1>
      <h2 class="text-2xl font-lexend text-amber-800 mt-9 mb-4">TAXES THAT WORK FOR YOU</h2>
      <p class="lg:text-lg text-base font-electolize font-extrabold  text-gray-800 lg:text-justify lg:mr-7">
Our taxes are split in Marketing (5%), LP (3%) and Burn (2%).

</p>
    </div>
     <div class="lg:inline-flex col-span-2 lg:flex-col  mt-10 py-12">
       <h2 class=" text-3xl font-lexend text-amber-800  uppercase">Total Supply</h2>
       <p class=" text-xl lg:text-2xl font-lexend font-extrabold text-gray-800 mt-4 ml-1">
 1,000,000,0000
</p>
 <p class=" text-base font-rubik font-extrabold text-gray-800 mt-1">
Monstrous Supply Gives us a Vision of killing More Zeros
</p>
  <div class="inline-flex  mt-6 ">
  <div class="lg:px-10 px-5">
    <radial-progress-bar :diameter="150"
                       :completed-steps="10"
                       :total-steps="100"
                       startColor ="#4b00a1"
                       stopColor ="#4b00a1"
                       innerStrokeColor ="#d1d1d1"
                       strokeWidth=17
                       innerStrokeWidth=15
                       strokeLinecap="square"
                       >
                       <h2 class="text-base font-lexend text-amber-800 mt-2">BUY TAX</h2>
    <p class=" text-xl font-lexend font-extrabold text-gray-800 mt-2 ml-1">{{ 10 }}%</p>
    </radial-progress-bar>
  </div>
  <div class="lg:px-10 mr-7">
   <radial-progress-bar :diameter="150"
                       :completed-steps="10"
                       :total-steps="100"
                       startColor="#a1001d"
                       stopColor ="##a1001d"
                       innerStrokeColor ="#d1d1d1"
                       strokeWidth=17
                       innerStrokeWidth=15
                       strokeLinecap="square"
                       >
                       <h2 class="text-base font-lexend text-amber-800 mt-2">SELL TAX</h2>
   <p class=" text-xl font-lexend font-extrabold text-gray-800 mt-2 ml-1">{{ 10 }}%</p>
  </radial-progress-bar></div></div>
  </div>
  </div>
  </section>

</template>

<script >
import { defineComponent } from 'vue'
import RadialProgressBar from 'vue-radial-progress'
// import HelloWorld from '@/components/HelloWorld.vue' // @ is an alias to /src

export default defineComponent({
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Tokenomics',
  components: {
    RadialProgressBar
  }
})
</script>
