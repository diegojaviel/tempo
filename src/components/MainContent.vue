<script setup>
import Button from './Button.vue';
</script>


<template>
  <div class="container">
    <div class="content">
      <div class="left-col">
        <h1>Discover the best coffee</h1>

        <p>Bean Scene is a coffee shop that provides you with quality coffee that helps boost your productivity and helps build your mood. Having a cup of coffee is good, but having a cup of real coffee is greater. There is no doubt that you will enjoy this coffee more than others you have ever tasted.</p>

        <Button>Learn More</Button>
      </div>
      <div class="right-col">
        <img src="../assets/img/coffee-mug.png" alt="coffee mug">
      </div>
    </div>
    
  </div>
  <img class="coffee-blast" src="../assets/img/coffee_blast.png" alt="">
</template>

<style scoped>

.container{
  padding: 10rem 8rem;
}

.content{
  display: flex;
  gap: 3.6rem;
  width: 100%;
  justify-content: center;
  align-items: center;
}

.left-col{
  display: flex;
  flex-direction: column;
  gap: 2.9rem;
  width: 58.5rem;
}

.left-col h1{
  color: #603809;
  font-size: 5.4rem;
  font-weight: 700;
}

.content img{
  width: 100%;
}

.coffee-blast{
  width: 498px;
  height: 272px;
  position: relative;
  transform-origin: 0 0;
  transform: rotate(0deg) scale(1, -1);
  object-fit: cover;
  top: 10rem;
  left: -10rem;
}

</style>