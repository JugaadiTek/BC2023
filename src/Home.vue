<script setup>
import NavBar from "./components/NavBar.vue";
import hero from "./components/hero.vue";
import newsletter from "./components/newsletter.vue";
import servicescard from "./components/servicescard.vue";
import FAQs from "./components/FAQs.vue";
import postfeed from "./components/postfeed.vue";
import artcont from "./components/artcont.vue";
import optionslice from "./components/optionslice.vue";
import optionsliceArt from "./components/optionsliceArt.vue";
import Postfeed from "./components/postfeed.vue";

import { ref } from 'vue';

//===================  NAVIGATION BAR JSON  =======================
//=================================================================
const navigations = ref([
  {
    component: "NavBar",
    alt: ["nogap", "darkbg"],
    sliceContent: [
      { label: "Solution", url: '' },
      { label: "Resources", url: '' },
      { label: "About Us", url: '' }
    ]
  },

])

//========================  FOOTER JSON  ==========================
//=================================================================

const footers = ref([
  {
    component: "newsletter",
    alt: [" nogap-bottom ", "lavanderbg"]
  },

])


//=================== OTHER COMPONENT JSON  =======================
//=================================================================

const slices = ref([

  {
    component: "hero",
    alt: ["nogap-top", "darkbg"],
    sliceContent: {
      title: "Made For The Market",
      discription: "BuyChain is the end-to-end supply chain management software built for the LBM industry. We unify and mobilizes your sales, inventory, and banking so that you can meet the demands of an increasingly volatile market.",
      imageurl: "https://placekitten.com/640/360",
      herobg: "/src/assets/BG Blank.jpg",
      sub_moduleHotspot: {
        type: "buttons",
        alt: [""],
        buttonlist: [{
          url: "notporn.com",
          text: "sometext",
          type: ["alt1", "class3", "animationX"]
        },
        {
          url: "notporn.com",
          text: "sometext",
          type: ["alt1", "class3", "animationX"]
        }]
      }
    }
  },

  {
    component: "hero",
    alt: [" lightbg"],
    sliceContent: {
      title: "LBM Operations Software",
      discription: "BuyChain’s end-to-end platform connects and informs every aspect of your business. The system integrates every facet of your operations, facilitating communication between departments and providing a holistic view of the entire enterprise. With real-time inventory management and shipping, AI driven sales order, and financial transparency, you can buy and sell faster, reduce risk and never miss a deal or market move again. ",
      imageurl: "https://placekitten.com/640/360",
      iconurl: [
        { icnurl: "src/assets/btn-xlrg-alt1.svg" },
        { icnurl: "src/assets/btn-xlrg-alt2.svg" },
        { icnurl: "src/assets/btn-xlrg-alt.svg" }
      ]
    }
  },
  {
    component: "optionslice",
    alt: ["darkbg", "nogap"],
    sliceContent: {
      boxycontent: [
        { item: "Inventory Management" },
        { item: "Risk Management" },
        { item: "Order Management" },
        { item: "User Permission & Security" },
        { item: "eProcurement & eCommerce" },
        { item: "Sales Optimisation" },
        { item: "Reporting & Optimization" },
        { item: "Shipping & Logistics" },
        { item: "Client & Account Management" },
        { item: "Finance & Accounting" },
      ],
    }
  },

  {
    component: "optionsliceArt",
    alt: [" lightbg"],
    sliceContent: {
      details: {
        tittle: "Inventory Management",
        discription: "Our system eliminates time now spent on internal cross-checking by providing all stakeholders real-time inventory data, informing both purchasing and sales on what to buy and what is available to sell. ",
        benlist: [
          { item: "Benifit" },
          { item: "Benifit" },
          { item: "Benifit" },
          { item: "Benifit" },
          { item: "Benifit" },
          { item: "Benifit" },
          { item: "Benifit" },
          { item: "Benifit" },
          { item: "Benifit" },
          { item: "Benifit" },

        ]
      }
    }
  },

  {
    component: "artcont",
    alt: [" lightbg"],
    sliceContent:
    {
      tittle: "Manage Voaltility and Reduce Risk",
      discription: "The BuyChain system eliminates longtime, industry-wide constraints on profitability and growth with the tools, control, and data you need to gain a competitive edge. We have married technology with customer service in a way that has not previously existed in our industry.",
      boxycontent: [
        {
          imgurl: "https://placekitten.com/640/360",
          tittle: "Buy",
          details: "BuyChain is the end-to-end supply chain management software for the LBM industry that unifies and mobilizes your team, sales, inventory, and banking in order to meet the demands of an increasingly volatile market.",
        },
        {
          imgurl: "https://placekitten.com/640/360",
          tittle: "Manage",
          details: "BuyChain is the end-to-end supply chain management software for the LBM industry that unifies and mobilizes your team, sales, inventory, and banking in order to meet the demands of an increasingly volatile market.",
        },
        {
          imgurl: "https://placekitten.com/640/360",
          tittle: "Sell",
          details: "BuyChain is the end-to-end supply chain management software for the LBM industry that unifies and mobilizes your team, sales, inventory, and banking in order to meet the demands of an increasingly volatile market.",
        }
      ]
    }

  },
  {
    component: "postfeed",
    alt: [" lightbg"],
    sliceContent:
    {
      tittle: "Recent Post",
      boxycontent: [
        {
          date: "01/01/1999",
          articletittle: " article tittle here",
          detail: "BuyChain is the end-to-end supply chain management software for the LBM industry that unifies and mobilizes your team, sales, inventory, and banking in order to meet the demands of an increasingly volatile market.",
          readmore_url: "https://www.w3schools.com/css/css_pseudo_elements.asp"
        },
        {
          date: "01/01/1999",
          articletittle: " article tittle here",
          detail: "BuyChain is the end-to-end supply chain management software for the LBM industry that unifies and mobilizes your team, sales, inventory, and banking in order to meet the demands of an increasingly volatile market.",
          readmore_url: "https://www.w3schools.com/css/css_pseudo_elements.asp"
        },
        {
          date: "01/01/1999",
          articletittle: " article tittle here",
          detail: "BuyChain is the end-to-end supply chain management software for the LBM industry that unifies and mobilizes your team, sales, inventory, and banking in order to meet the demands of an increasingly volatile market.",
          readmore_url: "https://www.w3schools.com/css/css_pseudo_elements.asp"
        }
      ]
    }
  },
  {
    component: "FAQs",
    alt: [" lightbg"],
    sliceContent: {
      tittle: " FAQs",
      items_list: [
        { question: " how to sjsdjfosijfooj kjdfglk fdgjl ? ", category: " warehouse" },
        { question: " how to sjsdjfosijfooj kjdfglk fdgjl ? ", category: " warehouse" },
        { question: " how to sjsdjfosijfooj kjdfglk fdgjl ? ", category: " warehouse" },
        { question: " how to sjsdjfosijfooj kjdfglk fdgjl ? ", category: " warehouse" },
        { question: " how to sjsdjfosijfooj kjdfglk fdgjl ? ", category: " warehouse" },
        { question: " how to sjsdjfosijfooj kjdfglk fdgjl ? ", category: " warehouse" }
      ]
    }

  },

  {
    component: "servicecard",
    alt: [" lightbg"],
    sliceContent: {
      tittle: "Replace your hammer with a nail gun.",
      sub_moduleHotspot: {
        type: "buttons",
        alt: [""],
        buttonlist: [{
          url: "notporn.com",
          text: "sometext",
          type: ["alt1", "class3", "animationX"]
        },
        {
          url: "notporn.com",
          text: "sometext",
          type: ["alt1", "class3", "animationX"]
        }]
      },
      boxycontent: [
        {
          sub_header: " operations ",
          sub_discription: "BuyChain’s end-to-end platform connects and informs every aspect of your business. The system digitizes your operations, facilitates communication between departments and provides a holistic view of the entire enterprise. ",
          category: " ",
          subtittle: "popular features",
          list_items: [
            { item: "Feature" },
            { item: "Feature" },
            { item: "Feature" },
            { item: "Feature" },

          ],
          sub_moduleHotspot: {
            type: "buttons",
            buttonlist: [
              {
                url: "https://mail.google.com/mail/u/0/#inbox",
                text: "Learn More",
                type: ["alt1", "class3", "animationX"]
              },
              {
                url: "https://mail.google.com/mail/u/0/#inbox",
                text: "Learn More",
                type: ["alt1", "class3", "animationX"]
              },

            ]
          },
        },
        {
          sub_header: " capital ",
          sub_discription: "BuyChain’s end-to-end platform connects and informs every aspect of your business. The system digitizes your operations, facilitates communication between departments and provides a holistic view of the entire enterprise. ",
          category: " BETA ",
          subtittle: "popular features",
          list_items: [
            { item: "Feature" },
            { item: "Feature" },
            { item: "Feature" },
            { item: "Feature" },
          ],
          btns: [
            { btntxt: "learn more", url: "https://www.w3schools.com/js/js_json_syntax.asp " },
            { btntxt: "join waitlist", url: " " }
          ]
        },
        {
          sub_header: " dashboard ",
          sub_discription: "BuyChain’s end-to-end platform connects and informs every aspect of your business. The system digitizes your operations, facilitates communication between departments and provides a holistic view of the entire enterprise. ",
          category: " FREE ",
          subtittle: "popular features",
          list_items: [
            { item: "Feature" },
            { item: "Feature" },
            { item: "Feature" },
            { item: "Feature" },
          ],
          btns: [
            { btntxt: "go to dash board", url: " " }
          ]
        }
      ]
    }
  },

])
</script>



<template>
  <header></header>
  <main class="devh-">

    <!---------------------- NAVIGATION BAR ---------------------->
    <nav class="mainNav nogap darkbg" v-for="navigationbar in navigations">
      <NavBar :navbtn="navigationbar.sliceContent" />
    </nav>



    <!---<div class="wrapper">-->
    <section v-for="(slice, index) in slices" :class="[slice.alt, slice.component]" :id="`section_` + index"
      :key="index">


      <!--  style="min-height:80vh; background-image:url('src/assets/BG Blank.jpg');background-size:cover;background-repeat:no-repeat;background-position:center center;"  -->
      <div v-if="slice.component == 'hero'">

        <hero :herocont="slice.sliceContent" />
      </div>

      <div :class="container" v-else-if="slice.component == 'optionsliceArt'">
        <optionsliceArt :optionsliceArtCont="slice.sliceContent" />
      </div>

      <div class="container" v-else-if="slice.component == 'optionslice'">
        <optionslice :optionsliceCont="slice.sliceContent" />
      </div>

      <div :class="container" v-else-if="slice.component == 'artcont'">
        <artcont :artcontent="slice.sliceContent" />
      </div>

      <div :class="container" v-else-if="slice.component == 'postfeed'">
        <postfeed :postfeedCont="slice.sliceContent" />
      </div>

      <div :class="container" v-else-if="slice.component == 'FAQs'">
        <FAQs :FAQcont="slice.sliceContent" />
      </div>

      <div :class="container" v-else-if="slice.component == 'servicecard'">
        <servicescard :servicecardCont="slice.sliceContent" />
      </div>

    </section>
  </main>

  <!-- ----------------------------- FOOTER ----------------------------- -->

  <footer class="container lavanderbg nogap-bottom">
    <newsletter />
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
