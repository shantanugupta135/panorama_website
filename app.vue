<template>
  <div>
    <Home />
  </div>
</template>
<script>
import { defineNuxtConfig } from "nuxt/config";
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
