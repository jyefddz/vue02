<template>
    <div>
        <p>商品总数{{ count }}</p>
        <button v-on:click="count++">+1</button>
        <button v-on:click="addFn">+1</button>
        <button v-on:click="addFn1(5)">+5</button>
        <button @click="subFn">-1</button>
        <button @click="clrFn">清空</button>
    </div>
</template>

<script>
export default {
    name: 'App',
    data() {
        return {
            count: 0
        }
    },
    methods: {
        addFn() {
            this.count++
        },
        addFn1(val) {
            this.count += val
        },
        subFn() {
            this.count--;
        },
        clrFn() {
            this.count = 0
        }
    }
}
</script>

<style>
</style>