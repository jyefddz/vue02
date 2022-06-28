<template>
  <div>
    {{ getSum() }}
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
    getSum() {
      let arr = [{ a: 100 }, { a: 20 }, { a: -10 }]
      const sum = arr.reduce((pre, curr) => {
        return pre + curr.a
      }, 0)
      console.log(sum);
    }
  }
}
</script>

<style>
</style>