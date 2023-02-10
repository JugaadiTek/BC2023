<script setup >
import NavBar from "./components/NavBar.vue";
import heroWithForm from "./components/heroWithForm.vue";
import heroWithForm2 from "./components/heroWithForm2.vue";
import articleHero from "./components/articleHero.vue";
import shortHero from "./components/shortHero.vue";
import articleBrick from "./components/articleBrick.vue";
import sidebarBrick from "./components/articleBrick.vue";
// import newsletter from "./components/newsletter.vue";
import footerSlice from "./components/footerSlice.vue";
import { ref } from 'vue';

//===================  NAVIGATION BAR JSON  =======================
//=================================================================
const navigations = ref([{ "component": "NavBar", "logo": { "type": "svg/img/text", "text": "", "altText": "", "logoFill": "" }, "alt": ["nogap", "darkbg"], "bricks": [{ "label": "Solution", "url": "" }, { "label": "Resources", "url": "" }, { "label": "About Us", "url": "" }], "buttons": [{ "type": "", "text": "", "url": "", "alt": [""], "external": true, "rel": [""] }] }])

//========================  FOOTER JSON  ==========================
//=================================================================
const footer = ref([{ "footerContent": { "footerType": ["nogap", "darkbg"], "footerBrand": [{ "url": "", "altText": " ", "maxheight": 60, "type": "string" }, { "label": "", "type": "string" }], "footerLinks": [{ "label": "Solution", "link_list": [{ "label": "Operations", "url": "", "external": true }, { "label": "Capital", "url": "", "external": true }, { "label": "Suppliars", "url": "", "external": true }, { "label": "Distributers", "url": "", "external": true }, { "label": "Retailers", "url": "", "external": true }] }, { "label": "Resources", "link_list": [{ "label": "Data Dashboard", "url": "", "external": true }, { "label": "News Room", "url": "", "external": true }, { "label": "Events", "url": "", "external": true }, { "label": "How to Guides", "url": "", "external": true }, { "label": "Customer Support", "url": "", "external": true }, { "label": "Investor Relations", "url": "", "external": true }] }, { "label": "About Us", "link_list": [{ "label": "FAQs", "url": "", "external": true }, { "label": "Security", "url": "", "external": true }, { "label": "Get In Touch", "url": "", "external": true }, { "label": "Our Team", "url": "", "external": true }, { "label": "Careers", "url": "", "external": true }] }, { "label": "Legal", "link_list": [{ "label": "Security Statement", "url": "", "external": true }, { "label": "Term & Conditions", "url": "", "external": true }, { "label": "Privacy Policy", "url": "", "external": true }, { "label": "Cookie Statement", "url": "", "external": true }] }] } }])


//=================== OTHER COMPONENT JSON  =======================
//=================================================================
const header = ref([

])
const articleTags = ref([

])

const article = ([

])
const sidebar = ([

])
</script>

<template>
  <main>

    <!---------------------- NAVIGATION BAR ---------------------->
    <nav class="mainNav nogap darkbg">
      <NavBar :navbtn="mainnav.data" />
    </nav>

    <!---------------------- Article Content ---------------------->
    <heroWithSlice :herocont="hero.data" />
    <shortHero :herocont="articleTags.data" />
    <div class="container">
      <div class="inner-container">
        <articleBrick :articleSliceCont="article"></articleBrick>
        <sidebarBrick :articleSliceCont="sidebar"></sidebarBrick>
      </div>
    </div>
  </main>

  <!-- ----------------------------- FOOTER ----------------------------- -->

  <footer class="container">
    <footerSlice :data="footer.data" />
  </footer>
</template>

<style>
.darkbg.hero {
  background-color: unset;
}

#section_0.hero {
  padding-top: var(--section-gap);
}

.hero .content-block div h2 {
  text-align: left;
}

.content .content-block img {
  margin: auto;
}

.content .content-block .flex img {
  width: unset;
}

.flex {
  display: flex;
  max-width: 100%;
}

.column {
  flex-direction: column;
}

.svg-btn-grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
}
</style>
