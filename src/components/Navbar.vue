<template>
  <header>
    <nav>
      <RouterLink to="/logo" id="logo-url">
        <img :src="logo" :alt="alt" id="logo" />
      </RouterLink>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/pedidos">Pedidos</RouterLink>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Navbar",
  props: ["logo", "alt"]
};
</script>
<style scoped>
html {
  margin: 0px;
}

nav {
  display: flex;
  background-color: rgba(255, 111, 111, 0.74);
  border-bottom: 2px solid rgb(0, 0, 0);
  margin: 0px;
  justify-content: flex-end;
}

#logo-url {
  padding: 10px;
  margin: auto;
  margin-left: 0;
}

#logo{
  width: 40px;
  height: 40px; 
}

nav a{
  color: white ;
  text-decoration: none;
  align-content: center;
  margin: 12px;
  transition: .1s;
}

nav a:hover{
  color: gray;
}
</style>
