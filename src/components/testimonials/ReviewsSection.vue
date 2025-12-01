<script setup>
import ReviewTestimonial from './ReviewTestimonial.vue';

const { testimonials } = defineProps({
  testimonials: null,
});
</script>

<template>
  <section class="reviews-section section-padding section-bg" id="section_4">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-lg-12 col-12 text-center mb-4 pb-lg-2">
          <em class="text-white">Reviews by Customers</em>

          <h2 class="text-white">Testimonials</h2>
        </div>

        <div class="timeline">
          <ReviewTestimonial v-for="(testimonial, index) of testimonials" :key="testimonial.author.name"
            :testimonial="testimonial" :index="index" />
        </div>
      </div>
    </div>
  </section>
</template>
