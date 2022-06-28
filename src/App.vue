<template>
  <div>
    {{ resolve() }}
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
    resolve() {
      const process = (url) => {
        const index1 = url.indexOf('?'),
          index2 = url.indexOf('#'),
          params = url.slice(index1 + 1, index2).split('&')
        return params.reduce((pre, curr) => {
          const [key, value] = curr.split('=')
          pre[key] = value
          return pre
        }, {})
      }
      console.log(process('http://www.baidu.com?name=zhangsan&age=18&sex=nan#'));
    }
  }
}
</script>

<style>
</style>