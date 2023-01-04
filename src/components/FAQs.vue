<script setup>
defineProps({
  FAQcont: []
})
</script>


<template>
      <div class="inner-container">
        <div class="content">
          <div class="content-block">
            <h2>
              {{ FAQcont.tittle }}
            </h2>
            <ul v-for=" ques in FAQcont.items_list">
              <li>
                <span class = "question">{{ ques.question }}</span>
                <span class = "category">{{ ques.category }}</span>
                <span class = "answer">Oh, you're gonna be in a coma, all right. I'm a monster. As you may or may not know, Lindsay and I have hit a bit of a rough patch. Steve Holt! Army had half a day.Well, what do you expect, mother? Well, what do you expect, mother? Did you enjoy your meal, Mom? You drank it fast enough. I'm half machine. I'm a monster It's a hug, Michael. I'm hugging you. Steve Holt! Army had half a day. We just call it a sausage.</span>
              </li>
            </ul>
          </div>
        </div>
      </div>
</template>

<style scoped>

h2{
  font-size: 48px;
  color: var(--ter-h2-clr);
}
span:first-of-type{
  font-size: 20px;
  font-weight: bold;
  color: var(--ter-h2-clr);
}
span:last-of-type{
  color: var(--ter-h2-clr);
}


li {
  border: 1px solid #e9e5f1;
  border-radius: 4px;
  padding: 20px;
  text-align: left;
  background-color: #f1eff6;
}

li>span:last-of-type {
  float: right;
}

.content-block>h2 {
  text-align: left;
}
</style>