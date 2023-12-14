<template>
  <div id="app">
    <HelloWorld v-bind:title="message"  v-bind:num="num" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  name: 'App',
  // 呼び出す子のコンポーネントを宣言
  components: {
    HelloWorld,
  },
  data(){
    return {
      message:'validate',
      num: 13,
    }
  }
}

</script>