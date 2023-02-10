<script setup>
defineProps({
  herocont: []
})
</script>


<template>
  <div class="inner-container">
    <div class="content">
      <div class="content-block">
        <div>
          <h2>{{ herocont.title }}</h2>
          <p>{{ herocont.description }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
h2 {
  text-align: left;
}
p {
  text-align: left;
}
/* .inner-container {
  background-image: url('src/assets/BG Blank.jpg');
} */
</style>