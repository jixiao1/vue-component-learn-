<template>
  <div id="box">
    <h1>{{title}}</h1>
    <h3>{{value}}</h3>
    <button @click="title='test';">按钮</button>
  </div>
</template>

<script>
export default {
  // 外部属性
  props: ["value"],
  // 为什么组件的data需要为函数返回一个对象
  // 为了在组件复用返回不同的对象
  data() {
    return {
      title: "这是组件"
    };
  },
  methods: {

  },
  components: {

  },
  watch: {

  },
  compouted: {

  },

  mounted() {
    console.log(this); //vue组件对象
  }
  //其他的所有配置项都一样
};
</script>

<style>
#box{
  background: red;
}
</style>