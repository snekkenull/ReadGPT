<template>
  <div class="form-control">
    <div class="form-container">
      <form action="">
        <button type="submit" class="search-btn">
                            <span>
                                <svg width="17" height="17" viewBox="0 0 17 17" fill="none" xmlns="http://www.w3.org/2000/svg">
                                    <path d="M16 16L12.4584 12.4521M14.4211 7.71053C14.4211 9.49027 13.7141 11.1971 12.4556 12.4556C11.1971 13.7141 9.49027 14.4211 7.71053 14.4211C5.93078 14.4211 4.22394 13.7141 2.96547 12.4556C1.707 11.1971 1 9.49027 1 7.71053C1 5.93078 1.707 4.22394 2.96547 2.96547C4.22394 1.707 5.93078 1 7.71053 1C9.49027 1 11.1971 1.707 12.4556 2.96547C13.7141 4.22394 14.4211 5.93078 14.4211 7.71053Z" stroke="white" stroke-width="2" stroke-linecap="round"/>
                                </svg>
                            </span>
        </button>
        <input type="text" placeholder="Atomic habits, Deep work, Einstein">
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheForm"
}
</script>

<style scoped>

.form-control {
  width: 100%;
  margin: 3.5rem auto;
}

.form-container {
  display: flex;
  justify-content: center;
}

.form-container form {
  width: 450px;
  height: 60px;
  display: flex;
  justify-content: flex-start;
  align-items: center;
  padding: 10px;
  box-sizing: border-box;
  background-color: white;
  border-radius: 100px;
  box-shadow:
      0px 2.7px 4.6px rgba(0, 0, 0, 0.02),
      0px 7.4px 11.1px rgba(0, 0, 0, 0.023),
      0px 15.1px 20.5px rgba(0, 0, 0, 0.024),
      0px 28.1px 35.2px rgba(0, 0, 0, 0.026),
      0px 51.7px 60.6px rgba(0, 0, 0, 0.031),
      0px 72px 105px rgba(0, 0, 0, 0.05)
;
}

.form-container form input {
  font-family: NeueHaasDisplay-Roman;
  letter-spacing: 0.25px;
  width: 90%;
  border: none;
  background: transparent;
  font-size: 1rem;
  outline: none;
  padding-left: 10px;
  box-sizing: border-box;
}

.search-btn {
  background-color: var(--primary-blue);
  border: none;
  width: 40px;
  height: 40px;
  border-radius: 50px;
  cursor: pointer;
}

</style>