<script setup>
import TitleSection from "@/components/TitleSection.vue";
import FeedbackCard from "./FeedbackCard.vue";
</script>

<template>
  <div>
    <TitleSection
      title="Our coffee perfection feedback"
      description="Our customers has amazing things to say about us"
    />
  </div>
  <FeedbackCard
    quote="Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset....."
    name="Jonny Thomas"
    role="Project Manager"
    image="@/assets/img/feedback-img-1.png"
  />
</template>

<style scoped></style>
