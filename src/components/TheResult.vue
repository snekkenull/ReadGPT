<template>
  <div v-if="results" class="result-container">
<!--    <div class="regenerate-btn">-->
<!--      <button>regenerate</button>-->
<!--    </div>-->

    <div class="results">
      <div class="results-container">
        <div class="result-text" v-for="result in results">{{ result }}</div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "TheResult",
  props: {
    results: {
      type: Array,
      required: false,
    },
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
  width: 920px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0 auto;
  flex-direction: column;
}

.results-container {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.result-text {
  font-family: NeueHaasDisplay-Roman;
  letter-spacing: 0.3px;
  font-size: 1.2rem;
  text-align: left;
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

@media only screen and (max-width: 1024px) {
  .results {
    width: 90%;
  }
}

</style>