<script setup>
import TheWelcome from '../components/TheWelcome.vue'
import Footer from "@/components/Footer.vue";
import Header from "@/components/Header.vue";
import { SpeedInsights } from "@vercel/speed-insights/next";
</script>

<template>
  <main>
<!--    <Header />-->
    <TheWelcome />
    <Footer />
    <SpeedInsights />
  </main>
</template>
