
<script>
  export default {
    data() {
      return {
        count: 0
      }
    },
    methods: {
      addToCount() {
        this.count++;
      },
      substructFromCount() {
        this.count--;
      }
    }
}
</script>
<template>
  <main>
    <div>
      <h4>The current count is ...</h4>
      <h1>{{ count }}</h1>
      <button @click="substructFromCount">-</button>
      <button @click="addToCount">+</button>
    </div>
  </main>
</template>

<style scoped>
main {
  background-color: aliceblue;
  width: 100vw;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

div {
  text-align: center;
}
</style>