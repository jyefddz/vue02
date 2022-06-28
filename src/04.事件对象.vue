<template>
    <div>
        <a @click="one" href="http://www.baidu.com">阻止去百度</a>
        <br>
        <span @click="two(1, $event)">阻止去百度</span>
    </div>
</template>

<script>
export default {
    name: 'App',
    data() {
        return {}
    },
    methods: {
        one(e) {
            console.log(e);
            e.preventDefault()
        },
        two(val, event) {
            console.log(val);
            console.log(event);
        }
    }
}
</script>

<style>
</style>