<script setup>

</script>

<template>
  <nav>
      <a href="/" class="branding">Tempo Cafe</a>

      <ul class="navbar-navigation">
        <li><RouterLink to="/">Home</RouterLink></li>
        <li><RouterLink to="/menu">Menu</RouterLink></li>
        <li><RouterLink to="/about">About</RouterLink></li>
        <li><RouterLink to="/contact">Contact</RouterLink></li>
      </ul>
  </nav>
</template>


<style scoped>
nav{
  display: flex;
  justify-content: space-between;
  align-items: center;
  
  width: 100%;
  padding: 2rem 10rem;
  position: absolute;
  margin: 0 auto;

  background-color: transparent;
  z-index: 10;
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

.navbar-navigation a{
  font-size: 1.4rem;
  transition: .3s;
}
.navbar-navigation a:hover{
  color: #F9C06A;
}



</style>