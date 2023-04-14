<template>
  <div class="header-text-container">
    <div class="title">
      <div>Find your next <span>favorite book</span> with <br> ReadGPT</div>
    </div>
    <div class="subtitle">
      <div>
        ReadGPT is a book recommendation app based on the books <br> you've read before
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheTitle"
}
</script>

<style scoped>

.header-text-container {
  margin-top: 80px;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
}

.title {
  font-size: 3rem;
  font-family: NeueHaasDisplay-Medium;
  text-align: center;
}

.title span {
  color: var(--primary-blue);
}

.subtitle {
  font-family: NeueHaasDisplay-Roman;
  letter-spacing: 0.25px;
  font-size: 1rem;
  text-align: center;
}

</style>