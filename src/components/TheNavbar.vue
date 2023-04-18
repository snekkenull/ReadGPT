<template>
  <div class="nav-container">
    <nav>
      <div class="nav-left">
        <div class="logo">
          <a href="/">
            <span>
                <img src="@/assets/image/logo.svg" alt="Logo">
            </span>
          </a>
        </div>
      </div>

      <div class="nav-right">
        <div class="github-logo">
          <a href="https://github.com/snekkenull/YueGPT" target="_blank">
            <span>
                <img src="@/assets/image/github-mark.svg" alt="Github logo">
            </span>
          </a>
        </div>
      </div>

    </nav>
  </div>
</template>

<script>
export default {
  name: "TheNavbar"
}
</script>

<style scoped>

.nav-container {
  width: 100%;
  height: 80px;
  background-color: var(--navbar-bg-color);
  border-bottom: 1px solid rgba(0, 0, 0, 0.5);
}

.nav-container nav {
  width: 1310px;
  height: 100%;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  width: 140px;
}

.logo img {
  width: 100%;
}

@media only screen and (max-width: 1350px) {
  .nav-container nav {
    width: auto;
    padding: 0 20px;
  }
}

</style>