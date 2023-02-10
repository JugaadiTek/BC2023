<script setup >
import NavBar from "./components/NavBar.vue";
import heroWithForm from "./components/heroWithForm.vue";
import heroWithForm2 from "./components/heroWithForm2.vue";
import shortHero from "./components/shortHero.vue";
import articleSlice from "./components/articleSlice.vue";
import newsletter from "./components/newsletter.vue";
import footerSlice from "./components/footerSlice.vue";
import { ref } from 'vue';

//===================  NAVIGATION BAR JSON  =======================
//=================================================================
const navigations = ref([
  {
    component: "NavBar",
    logo: {
      type: "svg/img/text",
      text: "",
      altText: "",
      logoFill: "",
    },
    alt: ["nogap", "darkbg"],
    bricks: [
      { label: "Solution", url: '' },
      { label: "Resources", url: '' },
      { label: "About Us", url: '' }
    ],
    buttons: [
      {
        type: "",
        text: "",
        url: "",
        alt: [""],
        external: true,
        rel: [""]
      }
    ]
  },

])

//========================  FOOTER JSON  ==========================
//=================================================================

const footer = ref([
  [
    {
      "footerContent": {
        "footerType": [
          "nogap",
          "darkbg"
        ],
        "footerBrand": [
          {
            "url": "",
            "altText": " ",
            "maxheight": 60,
            "type": "string"
          },
          {
            "label": "",
            "type": "string"
          }
        ],
        "footerLinks": [
          {
            "label": "Solution",
            "link_list": [
              {
                "label": "Operations",
                "url": "",
                "external": true
              },
              {
                "label": "Capital",
                "url": "",
                "external": true
              },
              {
                "label": "Suppliars",
                "url": "",
                "external": true
              },
              {
                "label": "Distributers",
                "url": "",
                "external": true
              },
              {
                "label": "Retailers",
                "url": "",
                "external": true
              }
            ]
          },
          {
            "label": "Resources",
            "link_list": [
              {
                "label": "Data Dashboard",
                "url": "",
                "external": true
              },
              {
                "label": "News Room",
                "url": "",
                "external": true
              },
              {
                "label": "Events",
                "url": "",
                "external": true
              },
              {
                "label": "How to Guides",
                "url": "",
                "external": true
              },
              {
                "label": "Customer Support",
                "url": "",
                "external": true
              },
              {
                "label": "Investor Relations",
                "url": "",
                "external": true
              }
            ]
          },
          {
            "label": "About Us",
            "link_list": [
              {
                "label": "FAQs",
                "url": "",
                "external": true
              },
              {
                "label": "Security",
                "url": "",
                "external": true
              },
              {
                "label": "Get In Touch",
                "url": "",
                "external": true
              },
              {
                "label": "Our Team",
                "url": "",
                "external": true
              },
              {
                "label": "Careers",
                "url": "",
                "external": true
              }
            ]
          },
          {
            "label": "Legal",
            "link_list": [
              {
                "label": "Security Statement",
                "url": "",
                "external": true
              },
              {
                "label": "Term & Conditions",
                "url": "",
                "external": true
              },
              {
                "label": "Privacy Policy",
                "url": "",
                "external": true
              },
              {
                "label": "Cookie Statement",
                "url": "",
                "external": true
              }
            ]
          }
        ]
      }
    }
  ]

])


//=================== OTHER COMPONENT JSON  =======================
//=================================================================

const slices = ref([


  {
    component: "shortHero",
    type: "halves/short/overlap",
    devnotes: {
      moduleIDs: [1, 9, 13, 25, 6, 22, 31, 34, 38, 40, 43],
      generalNotes: "",
      moduleSpecificNotes: [
        { id: 0, note: "" }
      ]
    },
    alt: ["nogap-top", "darkbg" ],
    bricks: {
      title: "Made For The Market",
      description: "BuyChain is the end-to-end supply chain management software built for the LBM industry. We unify and mobilizes your sales, inventory, and banking so that you can meet the demands of an increasingly volatile market.",
      bgImage: "src/assets/AdobeStock_504230989.jpeg",
      bgImageAltText: "its a background image",
    }
  },

  {
    component: "articleSlice",
    bricks: {
      wysiwyg: '<h2>article subtitle</h2> <p> Lorem ipsum dolor sit amet consectetur adipisicing elit.Ut laboriosam aliquid ducimus, nihil maiores asperiores in consequuntur officiis aliquam assumenda neque necessitatibus reiciendis repellat impedit illo exercitationem vel culpa quis. </p> <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut laboriosam aliquid ducimus, nihil maiores asperiores in consequuntur officiis aliquam assumenda neque necessitatibus reiciendis repellat impedit illo exercitationem vel culpa quis. </p>',
      atoms: [        
        { url: "https://www.flaticon.com", text: "Load More", type: "button", styleModifiers: "" }
      ]
    }
  },

  {
    component: "newsletter",
    devnotes: {
      moduleIDs: [8, 24, 33, 36, 45],
      generalNotes: "",
      moduleSpecificNotes: [
        { id: 0, note: "" }
      ]
    },
    alt: ["nogap", "lavanderBg"],
    embedCode: "",
    shortcode: "",
    content: ""
  }

])
</script>



<template>
  <header></header>
  <main class="devh-">

    <!---------------------- NAVIGATION BAR ---------------------->
    <nav class="mainNav nogap darkbg" v-for="navigationbar in navigations">
      <NavBar :navbtn="navigationbar.bricks" />
    </nav>


    <!---<div class="wrapper">-->
    <section v-for="(slice, index) in slices" :class="[slice.alt, slice.component]" :id="`section_` + index"
      :key="index">

      

      <div v-if="slice.component == 'shortHero'" >
        <shortHero :herocont="slice.bricks" />
      </div>

      <div :class="container" v-else-if="slice.component == 'articleSlice'">
        <articleSlice :articleSliceCont="slice.bricks" />
      </div>


      <div :class="container" v-else-if="slice.component == 'newsletter'">
        <newsletter />
      </div>

    </section>
  </main>

  <!-- ----------------------------- FOOTER ----------------------------- -->

  <footer class="container">
    <footerSlice />
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
