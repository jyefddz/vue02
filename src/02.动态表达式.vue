<template>
    <div>
        <a v-bind:href="href">点击去百度</a>
        <img v-bind:src="imgUrl" />
        <img :src="imgLocal" />
        <img src="./assets/logo.png" />
    </div>
</template>

<script>
import imgLocal from './assets/logo.png';
export default {
    name: 'App',
    data() {
        return {
            href: 'http://www.baidu.com',
            imgUrl:
                'http://yun.itheima.com/Upload/./Images/20210412/60741c11ab77b.jpg',
            imgLocal: imgLocal,
        };
    },
};
</script>
