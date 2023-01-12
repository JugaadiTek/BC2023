<script setup>
defineProps({
  optionsliceArtCont: []
})
</script>

<template>
  <div class="inner-container">
    <div class="content">
      <div class="content-block">
        <div>
          <h2> <i class="fa-solid fa-user"></i> {{ optionsliceArtCont.details.title }}</h2>
          <p>{{ optionsliceArtCont.details.description }}</p>
          <a href="">Demo</a>
        </div>
        <div>
          <ul>
            <li v-for="ghoul, index in optionsliceArtCont.details.dataList" :key="index">
              {{ ghoul.item }}
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
h2 {
  text-align: left;
}

ul {
  text-align: center;
  padding: unset;
}

a {
  display: inline-block;
  border: 4px solid #280071;
  background-color: #280071;
  color: #ffffff;
  border-radius: 4px;
  margin-top: 10px;
  padding: 2px 56px;
}

.content-block {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 10px;
  align-self: center;
  text-align: left;
}

.content-block>div:last-child {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 6px;
  background-color: #e9e5f1;
  padding: 60px;
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