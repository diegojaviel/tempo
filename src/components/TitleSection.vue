<script setup>
defineProps({
  title: String,
  description: String,
  color: String,
});
</script>

<template>
  <div class="section">
    <h1 v-if="title" class="title" :style="{ color: color }">{{ title }}</h1>
    <p v-if="description" class="description" :style="{ color: color }">
      {{ description }}
    </p>
  </div>
</template>

<style scoped>
.section {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-items: center;
}
.title {
  color: #442808;
  font-size: 5.4rem;
  font-weight: 700;
  margin-bottom: 1.6rem;
}
.description {
  font-size: 2rem;
  color: #707070;
  font-weight: 400;
  line-height: 3.4rem;
}
</style>
