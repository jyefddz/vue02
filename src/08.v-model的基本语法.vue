<template>
    <div>
        <input type="text" v-model="val" />
        <br />
        <input type="text" v-bind:value="val1" @input="inputFn" />
    </div>
</template>

<script>
export default {
    name: "App",
    data() {
        return {
            val: "",
            val1: "",
        };
    },
    methods: {
        inputFn(e) {
            console.log(e.target.value);
            this.val1 = e.target.value;
        },
    },
};
</script>

<style>
</style>