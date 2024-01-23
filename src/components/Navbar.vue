<script setup>

</script>

<template>
  <nav>
    <div class="container">
      <a href="/" class="branding">Tempo Cafe</a>

      <ul class="navbar-navigation">
        <li><RouterLink to="/">Home</RouterLink></li>
        <li><RouterLink to="/menu">Menu</RouterLink></li>
        <li><RouterLink to="/about">About</RouterLink></li>
        <li><RouterLink to="/contact">Contact</RouterLink></li>
      </ul>
    </div>
  </nav>
</template>


<style scoped>
nav{
  display: flex;
  flex-direction: row;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  background-color: transparent;
  z-index: 10;
}

.container{
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 2rem 10rem;
}
.branding{
  font-family: var(--font-primary);
  font-size: 3.5rem;
  font-weight: 400;
  color: #fff;
}

.navbar-navigation{
  list-style: none;
  display: flex;
  gap: 60px;
}

.navbar-navigation li{
  font-size: 1.4rem;
}



</style>