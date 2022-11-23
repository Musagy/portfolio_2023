<template>
  <header>
    <nav>
      <a :href="routes[0].path" id="logo" >
        <img src="/Logo.svg" alt="Logo" />
      </a>
      <menu>
        <a
          v-for="route in routes"
          :href="route.path"
          :class="'route' + (path === route.path ? ' active' : '')"
        >
          {{ route.name }}
        </a>
      </menu>
    </nav>
  </header>
</template>

<script setup lang="ts">
const { path } = defineProps({
  path: {
    type: String,
    required: true,
    default: "",
  },
})
type route = { path: string; name: string }
const routes: route[] = [
  { path: "/", name: "Inicio" },
  { path: "/about", name: "Sobre mi" },
  { path: "/portfolio", name: "Portafolio" },
]
</script>

<style scoped>
header {
  background: #1b181e;
  outline: black 10px solid;
  position: fixed;
  margin-top: -100px;
  width: 100%;
  z-index: 10;
  
  display: flex;
  justify-content: center;
}
header:before {
  content: "";
  width: 100%;
  outline: white 6px solid;
  position: absolute;
  pointer-events: none;
}
header, header:before{
  height: 90px;
}
nav {
  display: flex;
  max-width: 1080px;
  width: 100%;
  margin: 0 1rem;
  justify-content: space-between;
  align-items: center;
}
#logo, #logo img {
  height: 60px;
}
menu {
  display: flex;
  gap: 32px
}
.route {
  text-decoration: none;
  color: white;
  font-weight: 600;
  font-size: 1.5rem;
}
.active {
  color: #FCC969;
}
</style>
