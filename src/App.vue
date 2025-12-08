<script setup>
import AboutSection from './components/AboutSection.vue';
import BaristaSection from './components/BaristaSection.vue';
import ContactSection from './components/ContactSection.vue';
import HeroSection from './components/HeroSection.vue';
import MenuSection from './components/menu/MenuSection.vue';
import ReviewsSection from './components/testimonials/ReviewsSection.vue';
import SiteFooter from './components/SiteFooter.vue';
</script>

<template>
  <main>
    <HeroSection />
    <AboutSection />
    <BaristaSection />
    <MenuSection />
    <ReviewsSection />
    <ContactSection />
    <SiteFooter />
  </main>
</template>
