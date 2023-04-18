<template>
  <div class="header-text-container">
    <div class="title">
      <div>一本好書<span>且當知己</span><br>閲GPT</div>
    </div>
    <div class="subtitle">
      <div>
        鍵入您所喜愛的作家或作品名，<br>讓閲GPT爲您推薦。
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
  font-family: Iansui094-Regular;
  text-align: center;
}

.title span {
  color: var(--primary-blue);
}

.subtitle {
  font-family: Iansui094-Regular;
  letter-spacing: 0.25px;
  font-size: 1rem;
  text-align: center;
}

@media only screen and (max-width: 800px) {
  .title {
    font-size: 2.5rem;
  }
}

@media only screen and (max-width: 612px) {
  .title {
    font-size: 2rem;
  }
}

@media only screen and (max-width: 512px) {
  .title {
    width: 95%;
  }

  .subtitle {
    width: 95%;
  }
}

</style>