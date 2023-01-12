<script setup>
defineProps({
  optionsliceCont: []
})
</script>

<template>
  <!--<div class="inner-container">
    <div class="content">
      <div class="content-block">-->
  <ul>
    <li v-for="(tokyo, index) in optionsliceCont.gridItems" :key="index">
      <span> <i class="fa-solid fa-user"></i> {{ tokyo.item }}</span>
    </li>
  </ul>
  <!--</div>
    </div>
  </div>-->
</template>

<style scoped>
.content-block {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
}

li {}

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

.optionslice UL {
  DISPLAY: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
  width: 100%;
  margin: unset;
  padding: unset;
  border: 2px solid var(--primary-dark);
  box-sizing: border-box;
}

.optionslice UL li {
  border: 2px solid var(--primary-dark);
  display: inline-flex;
  flex-direction: column;
}

.optionslice UL li span {
  margin: auto;
  color: white;
  text-align: center;
  font-weight: var(--fw-medi);

}
</style>