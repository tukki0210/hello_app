<template>
  <div id="app">
    <HelloWorld v-bind:title="message" />
    <hr>
    <button class="btn btn-primary" v-on:click="doAction">change title</button>
    <Quiz quiz_text='これはサンプルです' />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import Quiz from './components/Quiz.vue';

export default {
  name: 'App',
  // 呼び出す子のコンポーネントを宣言
  components: {
    HelloWorld,
    Quiz
  },
  data(){
    return {
      message:'HELLO',
    }
  },
  methods:{
    doAction(){
      var input = prompt('new title:')
      this.message = input
    }
  }
}

</script>