<script setup>
defineProps({
  postfeedCont: []
})
</script>


<template>
  <div class="inner-container">
    <div class="content">
      <div class="content-block">
        <h2>{{ postfeedCont.tittle }}</h2>
        <div>
          <div v-for="cardcont in postfeedCont.boxycontent">
            <p>{{ cardcont.date }}</p>
            <h3>{{ cardcont.articletittle }}</h3>
            <p>{{ cardcont.detail }}</p>
            <a :href="postfeedCont.readmore_url">Read more ></a>
          </div>
        </div>
        <a :href="postfeedCont">Go To Newsroom</a>
      </div>
    </div>
  </div>
</template>

<style scoped>

h2 {
  color: #280071;
  font-size: 48px;
  margin-bottom: 50px;
}

h3 {
  font-size: 24px;
  color: #280071;
  margin: auto;
  margin-bottom: 20px;
}

h3+p {
  font-size: 20px;
}

p {
  margin: auto;
}
div.content-block {
  text-align: center;
}
.content-block>div {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 45px;
  text-align: left;
}

.content-block>div>div {
  border: 1px solid #e9e5f1;
  border-radius: 5px;
  padding: 50px 40px;
}

.content-block>div>div>a {
  display: inline-block;
  color: #280071;
  font-weight: bold;
  padding-top: 100px;
  align-self: center;
}

.content-block>a {
  display: inline-block;
  color: #280071;
  background-color: #e9e5f1;
  border: 2px solid #280071;
  margin-top: 35px;
  padding: 3px;
  border-radius: 4px;
  font-weight: bold;
}

@media (max-width: 800px) {
  .content-block>div {
    grid-template-columns: repeat(1, 1fr);
  }
}


</style>