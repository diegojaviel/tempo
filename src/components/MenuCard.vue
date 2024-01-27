<script setup>
import Button from './Button.vue';

defineProps({
  title: String,
  description: String,
  price: String,
  image: String
});

</script>


<template>
  <div class="menu-card">
    <img src="../assets/img/cappuccino.png" :alt="title" class="menu-card-image">
    <div class="menu-card-body">
      <h3 class="menu-card-title"> {{ title }}</h3>
      <p class="menu-card-text"> {{ description }}</p>
      <div class="menu-card-price">{{price}}</div>
      <Button class="menu-button">Order Now</Button>
    </div>
  </div>
</template>


<style scoped>
.menu-card{
  position: relative;
  background: #fff9f1;
  border-style: solid;
  border-color: rgba(249, 192, 106, 0.42);
  border-width: 1px;
  width: 280px;
  height: 364px;
}

.menu-card-image{
  width: 100%;
  object-fit: cover;
}

.menu-card-body{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-items: center;
}
.menu-card-title {
  color: #442808;
  margin-top: 1.4rem;
  font-size: 2.2rem;
  font-weight: 700;
}

.menu-card-text {
  color: #1e1e1e;
  font-size: 1.6rem;
  font-weight: 400;
}

.menu-card-price {
  color: #442808;
  font-size: 1.8rem;
  font-weight: 700;
  margin-bottom: 1.8rem;
}

.menu-button{
  position: absolute;
  bottom: -3rem;
  left: 50%;
  transform: translateX(-50%);
}
</style>