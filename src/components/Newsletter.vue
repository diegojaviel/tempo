<script setup>
import TitleSection from "./TitleSection.vue";
</script>

<template>
  <div class="newsletter-section">
    <TitleSection
      title="Subscribe to get the Latest News"
      description="Don’t miss out on our latest news, updates, tips and special offers"
      color="white"
    />
    <div class="input-wrap">
      <input
        type="email"
        v-model="email"
        placeholder="Enter your email"
        required
      />
      <button>Subscribe</button>
    </div>
  </div>
</template>

<style scoped>
.newsletter-section {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 2.5rem;

  margin-top: 10rem;
  height: 40rem;

  background-image: url("../assets/img/tempo-cafe-3.jpg.png");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
}

.input-wrap {
  display: flex;
  justify-content: center;
}

.input-wrap input {
  padding: 1.6rem 2rem;
  border: none;
  width: 55rem;
  border-top-left-radius: 0.4rem;
  border-bottom-left-radius: 0.4rem;
}
.input-wrap input:focus {
  outline: none;
}

button {
  color: #442808;
  font-size: 1.6rem;
  font-weight: 700;
  background: #f9c06a;
  padding: 1.8rem 2.4rem;
  border: none;
  border-top-right-radius: 0.4rem;
  border-bottom-right-radius: 0.4rem;
}
</style>
