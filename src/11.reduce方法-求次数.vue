<template>
    <div>
        {{ getNum() }}
    </div>
</template>

<script>
export default {
    name: "App",
    data() {
        return {

        }
    },
    methods: {
        getNum() {
            let str = 'hdshgvdvgebdhguedbhbweg'
            const strNum = str.split('').reduce((pre, cur) => {
                if (cur in pre) {
                    pre[cur]++
                }
                else {
                    pre[cur] = 1
                }
                return pre
            }, {})
            console.log(strNum);
        }
    }
}
</script>

<style>
</style>