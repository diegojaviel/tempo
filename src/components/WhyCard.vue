<script setup>

defineProps({
  title: String,
  description: String,
  image: String
});

</script>


<template>
  <div class="why-card">
    <div class="why-card-body">
      <img src="../assets/img/coffee-beans.png" :alt="title" class="why-card-image">
      <h3 class="why-card-title"> {{ title }}</h3>
      <p class="why-card-text"> {{ description }}</p>
    </div>
  </div>
</template>


<style scoped>
.why-card{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  background: #fff9f1;
  border-style: solid;
  border-color: rgba(249, 192, 106, 0.42);

  border-width: 1px;
  margin-top: 3.2rem;
  margin-bottom: 3.2rem;
}
.why-card-image{
  margin-bottom: 2.5rem;
}
.why-card-body{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 280px;
  height: 284px;
}

.why-card-title{
  color: #442808;
  font-size: 2.8rem;
  font-weight: 700;
}

.why-card-text{
  color: #707070;
  font-size: 2rem;
  font-weight: 400;
  text-align: center;
}
</style>