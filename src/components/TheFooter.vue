<script setup land="ts">
import { RouterLink } from "vue-router";
</script>

<template>
  <div class="py-5 text-center">
    <p>CMA CONNECT FAREHAM - Registered Charity Number 1182335</p>

    <p>
      5A Upper St Michael's Grove<br />
      PO14 1DN<br />
      Fareham<br />
    </p>

    <RouterLink to="privacy-policy">Privacy Policy →</RouterLink>
  </div>
  <div class="py-5 text-center bottom-line">
    <p>With the generous support of</p>
    <div class="flex flex-wrap justify-center">
      <img src="@/assets/support/allchurches.png" class="w-1/2 m-5" />
      <img src="@/assets/support/cinnamon_network.jpg" class="w-1/2 m-5" />
      <img src="@/assets/support/lottery.svg" class="w-1/2 m-5" />
      <img src="@/assets/support/love_portsmouth.png" class="w-1/2 m-5" />
      <img src="@/assets/support/the_well.jpg" class="w-1/4 m-5" />
    </div>
  </div>
</template>
