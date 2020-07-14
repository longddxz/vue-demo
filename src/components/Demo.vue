<template>
    <div id="firstDemo">
      <h1>{{demoDetail}}</h1>
      <h1>{{detail()}}</h1>
    </div>
</template>

<script>
  let newVar = {
    name: 'Demo',
    data: {
      demoDetail: 'demo详情'
    },
    methods: {
      detail: function () {
        return this.demoDetail
      }
    }
  }
  export default newVar
</script>

<style scoped>

</style>
