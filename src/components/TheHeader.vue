
<script setup lang="ts">
import { RouterLink } from "vue-router";
defineProps<{
  msg: string;
}>();
</script>

<template>
  <header class="bg-cmablue text-white">

    <RouterLink to="/">
      <img
        alt="CMA Connect Fareham logo"
        src="@/assets/CMA_connect_fareham_logo.png"
        align="center" 
        class="block mx-auto w-4/5"
      />
    </RouterLink>

    <nav class="">
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/how-we-can-help">How we can help</RouterLink>
      <RouterLink to="/who-we-are">Who we are</RouterLink>
      <RouterLink to="/support-us">Support us</RouterLink>
    </nav>
  
    <div class="">
      <p>Book a time to meet with our volunteer money mentors:</p>
      <ul>
        <li>
          Call <a href="tel:01329 284837" title="Call Us">01329 284837</a> 
        </li>
        <li>
          Email us at <a href="mailto:cmafareham@gmail.com" title="Email us">cmafareham@gmail.com</a></li>
        <li>
          Sign up to our<a href="https://www.facebook.com/cmaconnectfareham" title="CMA Connect Fareham Facebook page"> Facebook page</a>
        </li>
        </ul>
    </div>
  
  </header>
</template>
