<script setup>
import Navbar from './Navbar.vue';
import Button from './Button.vue';
</script>

<template>
  <Navbar/>
  <div class="overlay">
    <div class="hero">
    <h2>We’ve got your morning covered with</h2>

    <h1 class="title">Coffee</h1>
    <p>It is best to start your day with a cup of coffee. Discover the
    best flavours coffee you will ever have. We provide the best
    for our customers.</p>

    <Button>Order Now</Button>

    </div>
  </div>
  
</template>


<style scoped>

.overlay {
  position: relative;
  background: linear-gradient(89.82deg, rgba(30, 30, 30, 1.00) 0%,rgba(0, 0, 0, 0.00) 100%), url("../assets/img/hero-img.png") center/cover no-repeat;;
  width: 100%;
  height: 768px;
  position: relative;
}
.hero{
  position: absolute;
  background-size: cover;
  height: 80rem;
  width: 100%;
  padding-top: 15rem;
  padding-left: 10rem;
}
.title{
  font-family: var(--font-primary);
  font-size: 22rem;
  font-weight: 400;
  color: #fff;
}

h2{
  color: #fff;
  font-size: 2.2rem;
  font-weight: 500;
}

p{
  color: #fff;
  font-size: 2rem;
  line-height: 3.4rem;
  font-weight: 400;
  width: 572px;
  margin-bottom: 2rem;
}
</style>