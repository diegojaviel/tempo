<script setup>
defineProps({
  quote: String,
  name: String,
  role: String,
  image: String,
});
</script>

<template>
  <div class="feedback-container">
    <!-- <div class="navigation-arrow left-arrow">
      <img src="../assets/img/arrow-left.png" alt="Left arrow" />
    </div> -->
    <div class="feedback-content">
      <blockquote class="feedback-quote">
        <p>{{ quote }}</p>
      </blockquote>
      <div class="feedback-footer">
        <div class="feedback-person">
          <h4 class="feedback-name">{{ name }}</h4>
          <p class="feedback-role">{{ role }}</p>
        </div>
        <div class="feedback-image">
          <img src="../assets/img/feedback-img-1.png" alt="Person" />
        </div>

        <!-- <div class="navigation-arrow right-arrow">
          <img src="../assets/img/arrow-right.png" alt="Right arrow" />
        </div> -->
      </div>
    </div>
  </div>
</template>

<style scoped>
.feedback-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: 0 auto;

  background: #fff9f1;
  border-style: solid;
  border-color: rgba(249, 192, 106, 0.42);

  border-width: 1px;
  margin-top: 3.2rem;
  padding-bottom: 10rem;
  margin-bottom: 3.2rem;

  width: 98rem;
}
.feedback-content {
  text-align: center;
  padding-top: 13rem;
  position: relative;
}

.feedback-content::before {
  content: url("../assets/img/quote-icon.png");
  position: absolute;
  top: 5rem;
  left: 0;
  transform: translateX(-70%);
}
.feedback-quote {
  color: #707070;
  font-size: 1.8rem;
  line-height: 3.6rem;
  font-weight: 600;
  width: 780px;
  margin-bottom: 2.8rem;
}

.feedback-name {
  color: #442808;
  font-size: 3.2rem;
  font-weight: 700;
}

.feedback-role {
  color: #707070;
  font-size: 2rem;
  line-height: 3.4rem;
  font-weight: 400;
}

.feedback-image {
  position: absolute;
  bottom: -18rem;
  left: 50%;
  transform: translateX(-50%);
}
</style>
