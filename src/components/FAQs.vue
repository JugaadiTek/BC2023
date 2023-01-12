<script setup>
defineProps({
  FAQcont: []
})
</script>


<template>
  <div class="inner-container">

    <div class="content-block">
      <h2>
        {{ FAQcont.title }}
      </h2>
      <!-- <ul v-for=" ques in FAQcont.items_list">
              <li>
                <span class = "question">{{ ques.question }}</span>
                <span class = "category">{{ ques.category }}</span>
                <span class = "answer">Oh, you're gonna be in a coma, all right. I'm a monster. As you may or may not know, Lindsay and I have hit a bit of a rough patch. Steve Holt! Army had half a day.Well, what do you expect, mother? Well, what do you expect, mother? Did you enjoy your meal, Mom? You drank it fast enough. I'm half machine. I'm a monster It's a hug, Michael. I'm hugging you. Steve Holt! Army had half a day. We just call it a sausage.</span>
              </li>
            </ul> -->
      <!-- ========================================================== -->
      <div class="wrap-collabsible" v-for=" (ques, index) in FAQcont.items_list" key="index">
        <input :id="'collapsible2' + index" class="toggle" type="checkbox" checked="">
        <label :for="'collapsible2' + index" class="lbl-toggle">{{ ques.question }} <span><i
              class="fa-solid fa-user"></i></span> </label>

        <div class="collapsible-content">
          <div class="content-inner">
            <p>{{ ques.category }}</p>
          </div>
        </div>
      </div>
      <!-- ========================================================== -->
    </div>

  </div>
</template>

<style scoped>
h2 {
  font-size: 48px;
  color: var(--primary);
}

/* span:first-of-type{
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

li>span:nth-child(2) {
  float: right;
} */
.content-block {
  width: 100%;
}

.content-block>h2 {
  text-align: left;
}

/* ======================================================= */

input[type='checkbox'] {
  display: none;
}

.wrap-collabsible {
  margin: .1rem 0;

}

.lbl-toggle {
  display: block;
  font-weight: bold;
  font-family: monospace;
  font-size: 1.2rem;
  text-transform: uppercase;
  text-align: left;
  padding: 1rem;
  color: var(--primary);
  background: var(--bg-layer-300);
  border: 4px solid var(--bg-layer-600);
  cursor: pointer;
  border-radius: 7px;
  transition: all 0.25s ease-out;
}

.lbl-toggle:hover {
  color: var(--secondary);
}

.lbl-toggle::before {
  display: inline-block;
  border-top: 5px solid transparent;
  border-bottom: 5px solid transparent;
  border-left: 5px solid var(--bg-layer-600);
  vertical-align: middle;
  margin-right: .7rem;
  transform: translateY(-2px);
  transition: transform .2s ease-out;
}

.toggle:checked+.lbl-toggle::before {
  transform: rotate(90deg) translateX(-3px);
  border-bottom: unset;
}

.collapsible-content {
  max-height: 0px;
  overflow: hidden;
  transition: max-height .25s ease-in-out;
  min-width: 100%;
}

.toggle:checked+.lbl-toggle+.collapsible-content {
  max-height: 350px;
}

.toggle:checked+.lbl-toggle {
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
  border-bottom: unset;
  /* transition-delay: 5000ms; */
}

.collapsible-content .content-inner {
  background: var(--bg-layer-300);

  border-left: 4px solid var(--bg-layer-600);
  border-right: 4px solid var(--bg-layer-600);
  border-bottom: 4px solid var(--bg-layer-600);
  border-bottom-left-radius: 7px;
  border-bottom-right-radius: 7px;
  padding: .5rem 1rem;
}

.collapsible-content p {
  margin-bottom: 0;
}

label>span {
  float: right;
}
</style>