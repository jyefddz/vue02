<template>
  <div>
    <div>
      <span>年龄:</span>
      <input type="text" v-model.number="age">
    </div>
    <br>
    <div>
      <span>人生格言:</span>
      <input type="text" v-model.trim="motto">
    </div>
    <br>
    <div>
      <span>自我介绍:</span>
      <textarea cols="30" rows="10" v-model.lazy="intro"></textarea>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      age: '',
      motto: '',
      intro: ''
    }
  },
  methods: {

  }
}
</script>

<style>
</style>