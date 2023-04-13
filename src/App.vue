<template>
  <div class="main">
    <the-navbar/>
    <the-title/>
    <the-form/>
    <the-result/>
  </div>

  <div class="footer">
    <TheFooter/>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import TheNavbar from "@/components/TheNavbar.vue";
import TheFooter from "@/components/TheFooter.vue";
import TheTitle from "@/components/TheTitle.vue";
import TheForm from "@/components/TheForm.vue";
import TheResult from "@/components/TheResult.vue";

export default defineComponent({
  name: 'App',
  components: {TheResult, TheForm, TheTitle, TheFooter, TheNavbar},

});
</script>

<style>

:root {
  --navbar-bg-color: #E9E9E9;
  --bg-color: #F3F5F7;
  --primary-blue: #3086FD;
}

@font-face {
  font-family: 'NeueHaasDisplay-Bold';
  src: url('@/assets/fonts/NeueHaasDisplay-Bold.ttf');
}

@font-face {
  font-family: 'NeueHaasDisplay-Medium';
  src: url('@/assets/fonts/NeueHaasDisplay-Medium.ttf');
}

@font-face {
  font-family: 'NeueHaasDisplay-Roman';
  src: url('@/assets/fonts/NeueHaasDisplay-Roman.ttf');
}

html, body {
  margin: 0;
  padding: 0;
  background-color: var(--bg-color);
  font-size: 18px;
  height: 100%;
  min-height: 100vh;
  font-family: sans-serif, -apple-system, Arial, Helvetica, sans-serif, "Segoe UI", Roboto;
}

#app {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 100%;
}

</style>
