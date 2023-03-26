<template>
  <div>
    <Home />
  </div>
</template>
<script>
import { defineNuxtConfig } from "nuxt/config";
// importing AOS css style globally
import 'aos/dist/aos.css';
export default defineNuxtConfig({
  app: {
    head: {
      link: [
        {
          rel: "stylesheet",
          type: "text/css",
          href: "https://rsms.me/inter/inter.css",
        },
      ],
    },
  },
});
</script>
