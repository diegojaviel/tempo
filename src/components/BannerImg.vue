<script setup>
import Button from './Button.vue';

defineProps({
  backgroundUrl: String,
  title: String,
  description: String,
  bannerImg: String,
})
</script>

<template>
  <div class="banner-section">
    <div class="banner-text">
      <h1>{{ title }}</h1>
      <p>{{ description }}</p>
      <Button class="banner-btn">Order Now</Button>
    </div>
    <div class="banner-img">
      <img src="../assets/img/cup-img.png" alt="cup">
    </div>
  </div>
</template>

<style scoped>
.banner-section{
  display: flex;
  /* justify-items: center; */
  align-items: center;
  gap: 30rem;
  


  background-image: url("..//assets/img/banner-img.png") ;
  background-repeat: no-repeat;
  background-size: cover;
  width: 100%;
  height: 57.4rem;
  margin-bottom: 8rem;
}

.banner-section::before{
  content: '';
  background: #442808;
  opacity: 0.8;
  width: 100%;
  height: 574px;
  position: absolute;
}

.banner-text{
  display: flex;
  flex-direction: column;
  gap: 2.2rem;
  width: 57.5rem;
  margin-left: 10rem;
  position: relative;
  z-index: 1;
}
.banner-text h1{
  color: #ffffff;
  font-size: 5.4rem;
  font-weight: 700;
  margin-top: 13.5rem;
}

.banner-text p{
  color: #ffffff;
  font-size: 2rem;
  line-height: 3.4rem;
  font-weight: 400;
}

.banner-img{
  z-index: 1;
}

</style>