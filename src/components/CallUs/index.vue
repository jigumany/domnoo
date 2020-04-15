<template>
  <div class="call_us_container">
    <div class="container">

      <div
        class="first"
        v-scroll-reveal.reset="{delay:300,scarle:2}"
      >
        <h1>Hungry ?</h1>
      </div>
      <div
        class="second"
        v-scroll-reveal.reset="{delay:300,afterReveal:()=>{
          secondAnim = true
        }}"
      >
        <div v-if="secondAnim">
          <compAnim />
        </div>
      </div>
      <div
        class="third"
        v-scroll-reveal.reset="{delay:600,scarle:2}"
      >
        <span>Give Us A Call</span> <span>083 956 2134</span>
      </div>
    </div>
  </div>
</template>

<script>
import compAnim from "./anim.vue";

export default {
  data() {
    return {
      secondAnim: false
    };
  },
  components: {
    compAnim
  }
};
</script>