<template>
  <div class="result-container">
    <div class="regenerate-btn">
      <button>regenerate</button>
    </div>

    <div class="results">
      <div class="result-text" v-for="result in results" :key="result.id">{{ result.text }}</div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "TheResult",

  data() {
    return {
      results: [
        {id: 1, text: "1. Hard thing to hard things"},
        {id: 2, text: "2. Hard thing to hard things"},
        {id: 3, text: "3. Hard thing to hard things"},
        {id: 4, text: "4. Hard thing to hard things"},
        {id: 5, text: "5. Hard thing to hard things"},
        {id: 6, text: "6. Hard thing to hard things"},
        {id: 7, text: "7. Hard thing to hard things"},
      ],
    };
  },

})
</script>

<style scoped>

.result-container {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1.5rem;
}

.results {
  width: 1310px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0 auto;
  flex-direction: column;
  gap: 0.5rem;
}

.result-text {
  font-family: NeueHaasDisplay-Roman;
  letter-spacing: 0.3px;
  font-size: 1.2rem;
  text-align: center;
}

.regenerate-btn button {
  font-size: 1rem;
  font-family: NeueHaasDisplay-Roman;
  padding: 10px 20px;
  opacity: 0.5;
  cursor: pointer;
  border-radius: 50px;
  border: 1px solid rgba(0, 0, 0, 0.5);
  transition: all 0.2s ease;
}

.regenerate-btn button:hover {
  opacity: 1;
}

</style>