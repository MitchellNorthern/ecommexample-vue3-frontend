<template>
    <div>
        <button @click="incrementCounter">+</button>
        <div>{{ counter }}</div>
        <button @click="decrementCounter">-</button>
    </div>
</template>

<script>
import { ref } from '@vue/composition-api'

export default {
    setup() {
        /* ******* */
        /* COUNTER */
        /* ******* */
        const counter = ref(0)

        const incrementCounter = () => counter.value++
        const decrementCounter = () => counter.value--

        return {
            incrementCounter,
            decrementCounter,
            counter
        }
    }
}
</script>

<style></style>
