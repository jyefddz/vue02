<template>
    <div>
        <div>
            <span>用户名:</span>
            <input type="text" v-model="username">
        </div>
        <br>

        <div>
            <span>密码:</span>
            <input type="text" v-model="password">
        </div>
        <br>

        <div>
            <span>来自于:</span>
            <select v-model="from">
                <option value="北京市">北京</option>
                <option value="南京市">南京</option>
                <option value="天津市">天津</option>
            </select>
        </div>
        <br>

        <div>
            <span>爱好: </span>
            <input type="checkbox" v-model="hobby" value="抽烟">抽烟
            <input type="checkbox" v-model="hobby" value="喝酒">喝酒
            <input type="checkbox" v-model="hobby" value="写代码">写代码
        </div>
        <br>

        <div>
            <span>性别: </span>
            <input type="radio" value="男" name="sex" v-model="gender">男
            <input type="radio" value="女" name="sex" v-model="gender">女
        </div>
        <br>

        <div>
            <span>自我介绍</span>
            <textarea v-model="intro"></textarea>
        </div>
    </div>

</template>

<script>
export default {
    name: 'App',
    data() {
        return {
            username: '',
            password: '',
            from: '',
            hobby: [],
            gender: '',
            intro: ''
        }
    },
    methods: {

    }
}
</script>

<style>
</style>