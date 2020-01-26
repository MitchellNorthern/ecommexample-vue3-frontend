<template>
    <div>
        <button @click="incrementCounter">+</button>
        <div>{{ counter }}</div>
        <button @click="decrementCounter">-</button>
    </div>
</template>

<script>
import { ref } from 'vue'

export default {
    setup() {
        /* ************* */
        /* EXAMPLE STATE */
        /* ************* */
        const counter = ref(0)

        /* *************** */
        /* EXAMPLE METHODS */
        /* *************** */
        const incrementCounter = () => counter.value++
        const decrementCounter = () => counter.value--
    }
}
</script>

<style></style>
