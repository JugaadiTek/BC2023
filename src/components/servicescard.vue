<script setup>
defineProps({
  servicecardCont: []
})
</script>


<template>
  <div class="inner-container">
    <div class="content">
      <div class="content-block">
        <h2>{{ servicecardCont.title }}</h2>
        <p>{{ servicecardCont.description }}</p>
        <div>
          <div v-for="(cardcont, index) in servicecardCont.gridItems" :key="index">
            <p>{{ cardcont.category }}</p>
            <h3> <i class="fa-solid fa-user"></i> {{ cardcont.sub_header }}</h3>
            <p>{{ cardcont.description }}</p>
            <hr>
            <h4>{{ cardcont.subtitle }}</h4>
            <ul v-for="(items, index) in cardcont.itemsList" :key="index">
              <li> <i class="fa-solid fa-circle-check"></i> {{ items.item }}</li>
            </ul>
            <div v-for="(btton, index) in cardcont.atoms" :key="index">

              <a :href="btton.url" v-for="btn, index in btton " :key="index"> {{ btn.text }}</a>

            </div>

          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
h2 {
  margin-bottom: 48px;
}

h3 {
  margin: auto;
  margin-bottom: 30px;
}

h4 {
  margin: auto;
}

.content-block>div>div {
  padding: 45px 40px;
}



.content-block>div {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 45px;

}

.content-block>div>div {
  background-color: aliceblue;
  text-align: left;
  border: 1px solid #e9e5f1;
  border-radius: 5px;
}

hr {
  opacity: 60%;
}

.content-block>div>div>div {
  display: inline-block;
  padding-left: 1rem;
}

.content-block>div>div>div>a {
  color: #280071;
  border: 1.5px solid #280071;
  font-weight: bold;
  border-radius: 3px;
}

a {
  color: whitesmoke;
  font-weight: bold;
  background-color: #280071;
}

@media (max-width: 800px) {
  .content-block>div {
    grid-template-columns: repeat(1, 1fr);
  }
}
</style>