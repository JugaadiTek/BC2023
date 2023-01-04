<script setup>
defineProps({
  optionsliceCont: []
})
</script>

<template>
  <div class="inner-container">
    <div class="content">
      <div class="content-block">
        <ul v-for=" tokyo, index in optionsliceCont.boxycontent" :key="index">
          <li>{{ tokyo.item }}</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped>

.content-block {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr;  
}

li{
  
}

ul {
  margin: unset;
  padding: unset;
  padding: 8px 0;
}

@media (max-width: 600px) {
  .content-block {
    grid-template-columns: repeat(1, 1fr);
  }
}

@media (max-width: 400px) {
  .content-block {
    grid-template-columns: repeat(1, 1fr);
  }
}
</style>