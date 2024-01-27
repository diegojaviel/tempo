<script setup>

</script>


<template>
  <button>
    <slot></slot>
  
  </button>
</template>


<style scoped>

button{
  background: #f9c06a;
  border-radius: 2.4rem;
  width: 14rem;
  height: 5rem;
  position: relative;
  box-shadow: 0px 6px 12px 0px rgba(249, 192, 106, 0.22);
  cursor: pointer;
  font-size: 1.6rem;
  font-weight: 700;
  color: #1e1e1e;
  transition: .3s;
}

button:hover{
  background: #F1CA8E;
  color: #343434;
}


</style>