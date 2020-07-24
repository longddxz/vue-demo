<template>
    <div id="firstDemo">
      <ol>
        <!--循环-->
        <li v-for="nameVal in nameVals">
          {{ nameVal.nameVal }}
        </li>
        <li v-for="(index, key, val) in nameVals">
          {{ key }},{{val}},{{index}}
        </li>

        <!--if-else-->
        <div v-if="Math.random() > 0.5">
          ran大于0.5
        </div>
        <div v-else>
          ran 小于等于0.5
        </div>

        <el-dialog></el-dialog>

      </ol>
      <h1>{{demoDetail}}</h1>
      <h1>{{detail()}}</h1>
    </div>
</template>

<script>
let newVar = {
  name: 'Demo',
  data () {
    return {
      demoDetail: 'demo详情',
      nameVals: [
        {nameVal: 'lyj-1'},
        {nameVal: 'lyj-2'},
        {nameVal: 'lyj-3'}
      ]
    }
  },
  methods: {
    detail () {
      return this.demoDetail
    }
  }
}
export default newVar
</script>

<style scoped>

</style>
