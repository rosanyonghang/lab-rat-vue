<template>
  <div class="home">
   this is the home vview
<!--   <HelloWorld msg="hehehhe"/>-->
<!--   <HelloWorld :msg="word"/>-->
    <h2>Iterations</h2>
   <HelloWorld v-for="(word,index) in words" :key="index" :msg="word"/>
    <h2>Conditionals and methods</h2>
    <h1 class="vis" v-if="display">this should be visible</h1>
<!--    <input type="text" v-model="wordSingle"/>-->
<!--    <h1>{{wordSingle}}</h1>-->
    <button v-on:click="toggleDisplayHandler">Click</button>
    <h2>Computed</h2>
    <h1>{{addMr}}</h1>

  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "../components/HelloWorld";
export default {
  name: 'home',
  components: {
    HelloWorld
    },
  data(){
    return{
      wordSingle:'hello',
      words:['hehe','haha','huhu'],
      display:true,
      name:'Abiral',
      mrsWord:'Sangroula'
    }
  },
  methods:{
    toggleDisplayHandler(){
      this.display=!this.display
    }
  },
  mounted(){
  },
  computed:{
    addMr:function (){
      return 'mr '+ this.name
    }
  },

}
</script>
<style>

</style>
