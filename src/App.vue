<template>

  <Header />
  <Board />
  
</template>

<script>
import Header from "./components/Header.vue"
import Board from "./components/Board.vue"


export default{ 
  name: "App",
  components:{
    Header,
    Board
  }
}
</script>


<style>


</style>
