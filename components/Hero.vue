<template>
  <section id="hero" class="container-fluid">
    <div class="container">
      <div class="row">
        <div class="col col-md-8">
          <div class="left text-left">
            <h1>{{ heading }}</h1>
            <a :href="btnLink" class="button primary">{{ btnText }}</a>
          </div>
        </div>
        <div class="col col-md-4">
          <div class="right text-right">
            <img src="~/assets/img/home/hero-phone.png" alt="" srcset="" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  props: ["heading", "btnLink", "btnText"],
};
</script>