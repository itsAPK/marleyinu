/* eslint-disable new-cap */
/* eslint-disable @typescript-eslint/no-unused-consts */
/* eslint-disable no-undef */
// eslint-disable-next-line vue/multi-word-component-names
<template>
<section id="roadmap" style="background-color: #000000">
  <div class="lg:flex container  items-center justify-center p-10">
    <div class="inline-flex  col-span-3 flex-col m-1">
      <h1 class="text-6xl font-barlow uppercase font-extrabold text-amber-400 text-center mb-7">Roadmap</h1></div>
  </div>
  <main class="timeline-wrapper">
    <div class="svg-timeline">
     <svg width="8px" height="2490.7px" viewBox="0 0 8 2490.7">
        <line id="timeline" fill="none" stroke="#FFFFFF" stroke-width="8" stroke-miterlimit="10" x1="4" y1="0" x2="4" y2="2090.7"/>
      </svg>
    </div>
    <ol class="timeline clearfix">
      <li class="timeline__item">
        <div class="bg-amber-300 rounded-lg" style="background-color:#de9f00">
        <h3 class="text-4xl font-barlow text-amber-800 p-10">PHASE I</h3>
        <div class="block text-justify text-md text-gray-900 font-lexend400 font-extrabold px-16 pt-5 py-12">
              <p>-Stealth Launch </p>
              <p>-Website Development </p>
              <p>-Community building</p>
              <p>-MARKETING compaigns</p>
        </div></div>
      </li>
      <li class="timeline__item right">
         <div class="bg-amber-300 rounded-lg" style="background-color:#de9f00">
        <h3 class="text-4xl font-barlow text-amber-800 p-10">PHASE II</h3>
        <div class="block text-justify text-md text-gray-900 font-lexend400 font-extrabold px-16 pt-5 py-12">
              <p>-Giveaways </p>
              <p>-First geneneration NFT Sale</p>
              <p>-Exchange listing</p>
              <p>-Audit + KYC</p>
        </div></div>
      </li>
      <li class="timeline__item">
        <div class="bg-amber-300 rounded-lg" style="background-color:#de9f00">
        <h3 class="text-4xl font-barlow text-amber-800 p-10">PHASE III</h3>
        <div class="block text-justify text-md text-gray-900 font-lexend400 font-extrabold px-16 pt-5 py-12">
              <p>-Bigger Marketing </p>
              <p>-Second geneneration NFT Sale</p>
              <p>-Marley Swap</p>
              <p>-Charity donation</p>
        </div></div>
    </li>
    <li class="timeline__item right">
        <div class="bg-amber-300 rounded-lg" style="background-color:#de9f00">
        <h3 class="text-4xl font-barlow text-amber-800 p-10">PHASE IV</h3>
        <div class="block text-justify text-md text-gray-900 font-lexend400 font-extrabold px-16 pt-5 py-12">
              <p>-MDAO </p>
              <p>-CRO BRIDGE </p>
              <p>-FIFA Themed NFTs</p>
              <p>-Certik Audit</p>
        </div></div>
      </li>
    <li class="timeline__item">
        <div class="bg-amber-300 rounded-lg" style="background-color:#de9f00">
        <h3 class="text-4xl font-barlow text-amber-800 p-10">PHASE V</h3>
        <div class="block text-justify text-md text-gray-900 font-lexend400 font-extrabold px-16 pt-5 py-12">
              <p>-MPAD </p>
              <p>-Lambo Giveaway </p>
              <p>-MPet Brand</p>
              <p class="text-md text-center mt-6 uppercase font-lexend">Coming Soon!!!</p>
        </div></div>
    </li>
    </ol>
  </main>

</section>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Roadmap'
})
</script>

<style lang="scss">
*, *:before, *:after {
  box-sizing: inherit;
}

.right {
  float:right;
  width:100%
}
/* ====== MIXINS ===== */
// BEM selectors mixin
// block__element
@mixin e($element) {
  &__#{$element} {
    @content;
  }
}

// block__element--modifier
@mixin m($modifier) {
  &--#{$modifier}{
    @content;
  }
}
// Media queries mixin
$sm: 31.25em; // 500px
$md: 50em; // 800px
$lg: 75em; // 1200px
@mixin mq($break) {
  @if $break=="sm" {
    @media screen and ( min-width: $sm) {
      @content;
    }
  }
  @else if $break=="md" {
    @media screen and ( min-width: $md) {
      @content;
    }
  }
  @else if $break=="lg" {
    @media screen and ( min-width: $lg) {
      @content;
    }
  }
  @else {
    @media screen and ( min-width: $break) {
      @content;
    }
  }
}

// Variables
$font-family--primary: 'Open Sans';
$font-weight--light: 300;
$font-weight--norm: 400;
$font-weight--semi: 600;
$font-weight--bold: 700;
$font-weight--ultra: 900;
$orange: #FF9639;
// helpers
%center-text {
  text-align: center;
}

%center-align {
  margin: 0 auto;
}

html {
  font-family: $font-family--primary;
  font-size: 100%;
  @include mq(sm) {
    font-size: 105%;
  }
  @include mq(md) {
    font-size: 115%;
  }
  @include mq(lg) {
    font-size: 125%;
  }
}

// button styles
%btn {
  display: inline;
  text-decoration: none;
  padding: .45em 1.25em;
  text-transform: uppercase;
  font-weight: $font-weight--norm;
  letter-spacing: 1px;
  font-size: .75rem;
  border-radius: 25px;
  color: white;
  font-family: $font-family--primary;
  transition: all 250ms ease;
}

.btn--primary {
  border: 1px solid white;
  @extend %btn;
    &:hover {
    background-color: white;
    color: black;
  }
}

.poster {
  height: 100vh;
  width: 100%;
  background-position: center center;
  background-image: url("http://codepen.vincebrown.me/assets/images/snow-mountains.jpg");
  // .poster__heading
  @include e('heading') {
    @extend %center-text;
    @extend %center-align;
    width: 95%;
    color: white;
    padding-top: 5.5rem;
    font-weight: $font-weight--semi;
    font-size: 2em;
    transition: all 400ms ease;
    @include mq(sm) {
      font-size: 2.25em;
    }
    @include mq(md) {
      font-size: 2.75em;
    }
  }
  @include e('subheading') {
    @extend %center-text;
    display: block;
    font-size: .3em;
    letter-spacing: 5px;
    font-weight: $font-weight--norm;
    text-transform: uppercase;
    color: $orange;
    padding-top: .8em;
    margin-bottom: .6em;
  }
} // end .poster

// timeline
.btn--comments{
  @extend %btn;
  background-color: rgba(255,255,255,.4);
  border:none;
  font-size: .6em;
  &:hover {
    background-color: rgba(255,255,255,.6);
  }
}

.timeline-wrapper{
  position: relative;
   padding-bottom:1.5em;
  background:  rgba(255,255,255,0);
}
.svg-timeline {
  position: absolute;
  margin-left:50%;
  transform: translateX(-50%);
  display:none;
  @include mq(md) {
    display:block;
  }
}
.timeline {
  transition:all 250ms ease;
  width: 90%;
  margin: 0 auto;
  @include mq(sm) {
    width: 80%;
  }
  @include mq(md) {
    width: 95%;
  }
  @include e('item') {
    margin-bottom: 4em;
    clear:both;
    @include mq(md) {
      width: 40%;
    }
  }
  // .timeline__day
  @include e('day') {
    font-weight: $font-weight--semi;
    font-size: .9em;
    color:white;
    text-transform: uppercase;
    padding-bottom:.75em;
    span{
      font-weight: $font-weight--light;
      color:orange;
      text-transform: none;
    }
  }
  //.timeline__day-sum
  @include e('day-sum') {
    color:white;
    font-weight: $font-weight--light;
    font-size: .8em;
    display:block;
    margin-bottom:1.5em;
    line-height: 1.5;

  }

}

.clearfix:after {
     visibility: hidden;
     display: block;
     font-size: 0;
     content: " ";
     clear: both;
     height: 0;
     }
.clearfix { display: inline-block; }
/* start commented backslash hack \*/
* html .clearfix { height: 1%; }
.clearfix { display: block; }
/* close commented backslash hack */
</style>
