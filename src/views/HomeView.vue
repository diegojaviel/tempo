<script setup>
import Section from "@/components/Section.vue";
import TitleSection from "@/components/TitleSection.vue";
import MenuCard from "@/components/MenuCard.vue";
import WhyCard from "@/components/WhyCard.vue";
import Button from "@/components/Button.vue";
import BannerImg from "@/components/BannerImg.vue";
import Feedback from "@/components/Feedback.vue";
import Newsletter from "@/components/Newsletter.vue";
import Footer from "@/components/Footer.vue";

const menuItems = [
  {
    id: 1,
    title: "Cappuccino",
    description: "Coffee 50% | Milk 50%",
    price: "$8.50",
    image: "@/assets/img/cappuccino.png",
  },
  {
    id: 2,
    title: "Chai Latte",
    description: "Coffee 50% | Milk 50%",
    price: "$8.50",
    image: "@/assets/img/chai-latte.png",
  },
  {
    id: 3,
    title: "Macchiato",
    description: "Coffee 50% | Milk 50%",
    price: "$8.50",
    image: "@/assets/img/macchiato.png",
  },
  {
    id: 4,
    title: "Expresso",
    description: "Coffee 50% | Milk 50%",
    price: "$8.50",
    image: "@/assets/img/expresso.png",
  },
];

const whyItems = [
  {
    id: 1,
    title: "Supreme Beans",
    description: "Beans that provides\ngreat taste",
    image: "@/assets/img/coffee-beans.png",
  },
  {
    id: 2,
    title: "High Quality",
    description: "We provide the\nhighest quality",
    image: "@/assets/img/badge.png",
  },
  {
    id: 3,
    title: "Extraordinary ",
    description: "Coffee like you have\nnever tasted",
    image: "@/assets/img/coffee-cup.png",
  },
  {
    id: 4,
    title: "Affordable Price",
    description: "Our Coffee prices are\neasy to afford",
    image: "@/assets/img/best-price.png",
  },
];
</script>

<template>
  <main>
    <Section />

    <section class="menu-section">
      <TitleSection
        title="Enjoy a new blend of coffee style"
        description="Explore all flavours of coffee with us. There is always a new cup worth experiencing"
      />
      <div class="menu">
        <MenuCard
          v-for="item in menuItems"
          :key="item.id"
          :title="item.title"
          :description="item.description"
          :price="item.price"
          :image="item.image"
        />
      </div>
    </section>

    <section class="why">
      <TitleSection
        title="Why are we different?"
        description="We don’t just make your coffee, we make your day!"
      />

      <div class="why-cards">
        <WhyCard
          v-for="why in whyItems"
          :key="why.id"
          :title="why.title"
          :description="why.description"
          :image="why.image"
        />
      </div>

      <p>Great ideas start with great coffee, Lets help you achieve that</p>
      <h2>Get started today.</h2>

      <Button class="btn-why"> Join Us</Button>
    </section>

    <BannerImg
      title="Get a chance to have an Amazing morning"
      description="We are giving you are one time opportunity to experience a better life with coffee."
    />
    <Feedback />
    <Newsletter />
    <Footer />
  </main>
</template>

<style>
.menu-section {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-items: center;
  margin-bottom: 4rem;
}

.menu {
  display: flex;
  gap: 2rem;
  margin-top: 3.2rem;
}

.why {
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  padding-top: 8rem;
  align-items: center;
  justify-items: center;
}

.why-cards {
  display: flex;
  align-items: center;
  justify-items: center;
  gap: 2rem;
  white-space: pre;
}

.why h2 {
  margin-bottom: 2.4rem;
}

.btn-why {
  margin-bottom: 8rem;
}
</style>
