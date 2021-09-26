<template>
  <section id="statistics" class="container-fluid">
    <div class="container">
      <div class="row">
        <div class="stats text-center">
          <header class="text-center">
            <h1 class="text-white">Some counts that matters</h1>
            <h3 class="text-white">
              Our achievement in the journey depicted in numbers
            </h3>
          </header>
          <div class="row">
            <div
              class="col col-3-md
               stat"
              v-for="statistic in statistics"
              :key="statistic.id"
            >
              <p class="value text-white">{{ statistic.value }}</p>
              <p class="description text-white">{{ statistic.description }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  props: ["statistics"],
};
</script>