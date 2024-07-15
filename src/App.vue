<script setup>
import {ref} from "vue"

const count = ref(0)

const addToCount = () => {
    count.value++;
  }

  const subtractFromCount = () => {
    count.value--;
  }
</script>


<template>
    <main>
        <div>
            <h4>The Curerent count is ...</h4>
            <h1>
                {{ count }}
            </h1>
            <button @click="subtractFromCount()">-</button>
            <button @click="addToCount()">+</button>
        </div>
    </main>
</template>

<style scoped>
main {
    background-color: aquamarine;
    widows: 100vw;
    height: 100vh;
    display: grid;
    place-items: center;
}
div {
    text-align: center;
}
</style>
