<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import HeaderInfo from "./components/HeaderInfo.vue";
</script>

<template>
  <div class="flex items-stretch my-8 mx-auto max-w-screen-2xl rounded-lg border">
    <header class="bg-cmablue basis-1/3 ">
      <img
        alt="CMA Connect Fareham logo"
        src="@/assets/CMA_connect_fareham_logo.png"
        align="center" 
      />

      <div class="wrapper">
        <HeaderInfo msg="You did it!" />

        <nav>
          <RouterLink to="/">Home</RouterLink>
          <RouterLink to="/about">About</RouterLink>
        </nav>
      </div>
    </header>
    <div class="basis-2/3">
      <RouterView />
    </div>
  </div>
</template>
