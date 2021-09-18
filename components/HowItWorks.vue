<template>
  <section id="howitworks">
    <div class="container">
      <div class="row">
        <div class="col-12 text-center header">
          <h1>How it works</h1>
        </div>
        <div class="col col-md-4 step" v-for="step in steps" :key="step.id">
          <img :src="step.image" alt="" srcset="" />
          <h2>{{ step.value }}</h2>
          <p>{{ step.description }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  props: ["steps"],
};
</script>