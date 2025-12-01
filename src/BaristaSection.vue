<script setup>
import BaristaPerson from './BaristaPerson.vue';

const { people } = defineProps({
  people: null,
});
</script>

<template>
  <section class="barista-section section-padding section-bg" id="barista-team">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-lg-12 col-12 text-center mb-4 pb-lg-2">
          <em class="text-white">Creative Baristas</em>

          <h2 class="text-white">Meet People</h2>
        </div>

        <BaristaPerson v-for="person in people" :key="person.name + person.tag" :person="person"/>
      </div>
    </div>
  </section>
</template>
