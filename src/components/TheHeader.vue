<script setup lang="ts">
  import { RouterLink } from "vue-router"
  import { ref } from  'vue'
  const menuOpen = ref(true)
  const toggleMenu = () => {
    menuOpen.value = !menuOpen.value
    console.log(menuOpen)
  }
</script>

<template>
  <header class="bg-cmablue text-white relative">
    <button
      :class="{ hidden: !menuOpen }"
      class="block fixed right-2 top-2"
      @click="toggleMenu"
    >
      <img src="@/assets/menu.svg" alt="open menu" />
    </button>
    <button
      :class="{ hidden: menuOpen }"
      class="block fixed right-2 top-2"
      @click="toggleMenu"
    >
      <img src="@/assets/close.svg" alt="clos menu" />
    </button>

    <RouterLink to="/">
      <img
        alt="CMA Connect Fareham logo"
        src="@/assets/CMA_connect_fareham_logo.png"
        align="center"
        class="block mx-auto w-3/4"
      />
    </RouterLink>

    <nav 
      :class="{ hidden: menuOpen}"
      class="absolute top bg-cmablue block w-full px-4 pb-2"
      >
      <RouterLink class="menu-item border-b" @click="toggleMenu" to="/">Home</RouterLink>
      <RouterLink class="menu-item border-b" @click="toggleMenu" to="/how-we-can-help">How we can help</RouterLink>
      <RouterLink class="menu-item border-b" @click="toggleMenu" to="/who-we-are">Who we are</RouterLink>
      <RouterLink class="menu-item" @click="toggleMenu" to="/support-us">Support us</RouterLink>
    </nav>

    <div class="hidden">
      <p>Book a time to meet with our volunteer money mentors:</p>
      <ul>
        <li>
          Call <a href="tel:01329 284837" title="Call Us">01329 284837</a>
        </li>
        <li>
          Email us at
          <a href="mailto:cmafareham@gmail.com" title="Email us"
            >cmafareham@gmail.com</a
          >
        </li>
        <li>
          Sign up to our<a
            href="https://www.facebook.com/cmaconnectfareham"
            title="CMA Connect Fareham Facebook page"
          >
            Facebook page</a
          >
        </li>
      </ul>
    </div>
  </header>
</template>
