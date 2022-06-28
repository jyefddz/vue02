<template>
    <div>
        <input type="text" @keydown.enter="enterFn">
        <br>
        <input type="text" @keydown.esc="escFn">
    </div>
</template>

<script>
export default {
    name: 'App',
    data() {
        return {

        }
    },
    methods: {
        enterFn() {
            console.log("enter");
        },
        escFn() {
            console.log("esc");
        }
    }
}
</script>

<style>
</style>