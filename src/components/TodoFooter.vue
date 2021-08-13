<template>
  <div class="clearAllContainer" @click="clearTodo" >
    <span class="clearAllBtn" >Clear All</span>
  </div>
</template>

<script>
export default {
  methods:{
    clearTodo(){
     this.$emit('removeAll')
    }
  }
}
</script>

<style>
  .clearAllContainer{
    width: 8.5rem;
    height: 50px;
    line-height: 50px;
    background-color: rgb(15, 228, 111);
    border-radius: 10px;
    margin: 0 auto;
  }
  .clearAllBtn{
    color:white;
    display:black;
  }
</style>