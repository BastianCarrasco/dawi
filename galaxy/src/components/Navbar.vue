<template>
  <nav>
    <ul>
      <li>
        <router-link to="/">Inicio</router-link>
      </li>
      <li>
        <router-link to="/about">Acerca de</router-link>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style scoped>
nav {
  background-color: #2c3e50;
  padding: 1rem;
}

ul {
  list-style: none;
  display: flex;
  gap: 1rem;
  margin: 0;
  padding: 0;
}

a {
  color: white;
  text-decoration: none;
}

.router-link-active {
  font-weight: bold;
  text-decoration: underline;
}
</style>