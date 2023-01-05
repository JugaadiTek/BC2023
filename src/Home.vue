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
import split_ImgTxt from "./components/split_ImgTxt.vue";
import footerSlice from "./components/footerSlice.vue";

import { ref } from 'vue';

//===================  NAVIGATION BAR JSON  =======================
//=================================================================
const navigations = ref([
  {
    component: "NavBar",
    logo: {
      type:"svg/img/text",
      text:"",
      altText:"",
      logoFill:"",
    },
    alt: ["nogap", "darkbg"],
    sliceContent: [
      { label: "Solution", url: '' },
      { label: "Resources", url: '' },
      { label: "About Us", url: '' }
    ],
    buttons: [
      {
        type:"",
        text:"",
        url:"",
        alt:[""],
        external:true,
        rel:[""]
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
    component: "hero",
    type: "halves/short/overlap",
    devnotes: {
      moduleIDs: [1, 9, 13, 25, 6, 22, 31, 34, 38, 40, 43],
      generalNotes: "",
      moduleSpecificNotes: [
        { id: 0, note: "" }
      ]
    },
    alt: ["nogap-top", "darkbg"],
    sliceContent: {
      brandLogo: [{ url: "url/url", altText: "text" }],
      title: "Made For The Market",
      discription: "BuyChain is the end-to-end supply chain management software built for the LBM industry. We unify and mobilizes your sales, inventory, and banking so that you can meet the demands of an increasingly volatile market.",
      imageurl: "https://placekitten.com/640/360",
      herobg: "/src/assets/BG Blank.jpg",
      herobgAltText: "",
      sub_moduleHotspot: [
        {
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
        {
          type: "iconbutton",
          alt: [""],
          buttonlist: [{
            url: "notporn.com",
            iconurl: "/url",
            text: "sometext",
            altText: "text",
            type: ["alt1", "class3", "animationX"]
          },
          {
            url: "notporn.com",
            text: "sometext",
            type: ["alt1", "class3", "animationX"]
          }]
        }

      ]
    }
  },
  {
    component: "ctaHero",
    // component: "blockquoteSlider",
    alt: ["fullwidth darkbg"],
    backgroundImage: "",
    devnotes: {
      moduleIDs: [4, 19, 28],
      generalNotes: "",
      moduleSpecificNotes: [
        { id: 0, note: "" }
      ]
    },
    sliceContent: [
      {
        icon: "fontawesomeIcon",
        rating: 5,
        quote: "header txt",
        attribution: "firstname lastname",
        jobTitle: "software engineer"
      }
    ]
  },
  {
    component: "singleimage",
    devnotes: {
      module: [26, 0],
      generalNotes: "",
      moduleSpecificNotes: [
        { module: 0, note: "" }
      ]
    },
    imageurl: "url",
    altText: "randommtext",
    linkurl:""

  },
  {
    component: "split_ImgTxt",
    devnotes: {
      module: [3, 11, 14, 18, 20, 37],
      generalNotes: "",
      moduleSpecificNotes: [
        { module: 0, note: "" }
      ]
    },
    alt: ["nogap-top", ""],
    sliceContent: {
      brandLogo: [{ url: "url/url", altText: "text" }],
      title: "Made For The Market",
      contentBlocks: [
        {
          discription: "description example",
          sub_moduleHotspot: [
            {
              type: "buttons", alt: [""], buttonlist: 
              [
                { url: "https://placekitten.com/640/360", text: "text 1", type: ["alt1", "class3", "animationX"] },
                { url: "https://placekitten.com/640/360", text: "text 1", type: ["alt1", "class3", "animationX"] },
                { url: "https://placekitten.com/640/360", text: "text 1", type: ["alt1", "class3", "animationX"] }
              ]
            },
            //, devnotes: { modules: [3, 0], note: "always 3 icon buttons" }
            {
              type: "iconbutton", alt: [""], devnotes: {
                modules: [3, 0], note: "always 3 icon buttons"}, buttonlist: 
             [
                { 
                  url: "https://placekitten.com/640/360", iconurl: "/url", altText: "text", 
                  type: ["alt1", "class3", "animationX"] 
                },
                { 
                  url: "https://placekitten.com/640/360", iconurl: "/url", altText: "text", 
                  type: ["alt1", "class3", "animationX"] 
                },
                  {
                    url: "https://placekitten.com/640/360", iconurl: "https://placekitten.com/640/360", altText: "text",
                    type: ["alt1", "class3", "animationX"]
                  }
              ]
            }
          ]
        }
      ],
      imageurl: "https://placekitten.com/640/360",
      imaAbs: [
        {imgabUrl:"",top:0,left:0,height:"",width:""},
      ]
    }
  },

  {
    component: "hero",
    // component:"halves",
    alt: ["lightbg"],
    sliceContent: {
      title: "LBM Operations Software",
      discription: "BuyChain’s end-to-end platform connects and informs every aspect of your business. The system integrates every facet of your operations, facilitating communication between departments and providing a holistic view of the entire enterprise. With real-time inventory management and shipping, AI driven sales order, and financial transparency, you can buy and sell faster, reduce risk and never miss a deal or market move again. ",
      imageurl: "https://placekitten.com/640/360",
      iconurl: [
        { icnurl: "src/assets/btn-xlrg-alt1.svg", altText: "text" },
        { icnurl: "src/assets/btn-xlrg-alt2.svg", altText: "text" },
        { icnurl: "src/assets/btn-xlrg-alt.svg", altText: "text" }
      ]
    }
  },
  {
    component: "optionslice",
    devnotes: {
      module: [15, "38a", 41],
      generalNotes: "",
      moduleSpecificNotes: [
        { module: 0, note: "" }
      ]
    },
    alt: ["darkbg", "nogap"],
    sliceContent: {
      boxycontent: [
        { item: "Inventory Management", icon: "fontawesomeIcon" },
        { item: "Risk Management", icon: "fontawesomeIcon" },
        { item: "Order Management", icon: "fontawesomeIcon" },
        { item: "User Permission & Security", icon: "fontawesomeIcon" },
        { item: "eProcurement & eCommerce", icon: "fontawesomeIcon" },
        { item: "Sales Optimisation", icon: "fontawesomeIcon" },
        { item: "Reporting & Optimization", icon: "fontawesomeIcon" },
        { item: "Shipping & Logistics", icon: "fontawesomeIcon" },
        { item: "Client & Account Management", icon: "fontawesomeIcon" },
        { item: "Finance & Accounting", icon: "fontawesomeIcon" }
      ]
    }
  },

  {
    component: "optionsliceArt",
    devnotes: {
      module: [16],
      generalNotes: "",
      moduleSpecificNotes: [
        { module: 0, note: "" }
      ]
    },
    alt: ["lightbg"],
    sliceContent: {
      details: {
        tittle: "Inventory Management",
        icon:"fontawesomeIcon",
        discription: "Our system eliminates time now spent on internal cross-checking by providing all stakeholders real-time inventory data, informing both purchasing and sales on what to buy and what is available to sell. ",
        //benlist: [[{ icon: "fontawesomeIcon", item: "Benifit" }], [{ icon: "fontawesomeIcon", item: "Benifit" }]] 
        benlist: [ 
          { icon:"fontawesomeIcon", item: "Benifit" },
          { icon:"fontawesomeIcon", item: "Benifit" },
          { icon:"fontawesomeIcon", item: "Benifit" },
          { icon:"fontawesomeIcon", item: "Benifit" },
          { icon:"fontawesomeIcon", item: "Benifit" },
          { icon:"fontawesomeIcon", item: "Benifit" },
          { icon:"fontawesomeIcon", item: "Benifit" },
          { icon:"fontawesomeIcon", item: "Benifit" },
          { icon:"fontawesomeIcon", item: "Benifit" },
          { icon:"fontawesomeIcon", item: "Benifit" }
        ]
      }
    }
  },

  {
    component: "artcont",
    devnotes: {
      module: [5, 10, 17, 27],
      generalNotes: "",
      moduleSpecificNotes: [
        { module: 0, note: "" }
      ]
    },
    alt: ["lightbg"],
    sliceContent:
    {
      tittle: "Manage Voaltility and Reduce Risk",
      discription: "The BuyChain system eliminates longtime, industry-wide constraints on profitability and growth with the tools, control, and data you need to gain a competitive edge. We have married technology with customer service in a way that has not previously existed in our industry.",
      boxycontent: [
        {
          imgurl: "https://placekitten.com/640/360",
          altText: "",
          tittle: "Buy",
          details: "BuyChain is the end-to-end supply chain management software for the LBM industry that unifies and mobilizes your team, sales, inventory, and banking in order to meet the demands of an increasingly volatile market.",
          buttonlist: [
            { url: "/url", text: "text" }
          ]
        },
        {
          imgurl: "https://placekitten.com/640/360",
          altText: "",
          tittle: "Manage",
          details: "BuyChain is the end-to-end supply chain management software for the LBM industry that unifies and mobilizes your team, sales, inventory, and banking in order to meet the demands of an increasingly volatile market.",
          buttonlist: [
            { url: "/url", text: "text" }
          ]
        },
        {
          imgurl: "https://placekitten.com/640/360",
          altText: "",
          tittle: "Sell",
          details: "BuyChain is the end-to-end supply chain management software for the LBM industry that unifies and mobilizes your team, sales, inventory, and banking in order to meet the demands of an increasingly volatile market.",
          buttonlist: [
            { url: "/url", text: "text" }
          ]
        }
      ]
    }

  },
  {
    component: "postfeed",
    devnotes: {
      module: [7, 23, 32, 35, 39, 44],
      generalNotes: "",
      moduleSpecificNotes: [
        { module: 0, note: "" }
      ]
    },
    alt: ["lightbg"],
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
    devnotes: {
      module: [21, 30, 42],
      generalNotes: "",
      moduleSpecificNotes: [
        { module: 0, note: "" }
      ]
    },
    alt: ["lightbg"],
    sliceContent: {
      tittle: "FAQs",
      items_list: [
        { question: "how to sjsdjfosijfooj kjdfglk fdgjl ?", icon:"fontawesomeIcon", content: "randomtext" },
        { question: "how to sjsdjfosijfooj kjdfglk fdgjl ?", icon:"fontawesomeIcon", content: "randomtext" }
      ]
    }

  },
  {
    component: "servicecard",
    devnotes: {
      module: [2, 12, 29],
      generalNotes: "",
      moduleSpecificNotes: [
        { module: 0, note: "" }
      ]
    },
    alt: ["lightbg"],
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
          icon: "fontawesomeIcon",
          sub_discription: "BuyChain’s end-to-end platform connects and informs every aspect of your business. The system digitizes your operations, facilitates communication between departments and provides a holistic view of the entire enterprise. ",
          category: " ",
          subtittle: "popular features",
          list_items: [
            { icon:"fontawesomeIcon", item: "Feature" },
            { icon:"fontawesomeIcon", item: "Feature" },
            { icon:"fontawesomeIcon", item: "Feature" },
            { icon:"fontawesomeIcon", item: "Feature" }
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
              }
            ]
          }
        },
        {
          sub_header: "capital",
          icon: "fontawesomeIcon",
          sub_discription: "BuyChain’s end-to-end platform connects and informs every aspect of your business. The system digitizes your operations, facilitates communication between departments and provides a holistic view of the entire enterprise. ",
          category: "BETA",
          subtittle: "popular features",
          list_items: [
            { icon:"fontawesomeIcon", item: "Feature" },
            { icon:"fontawesomeIcon", item: "Feature" },
            { icon:"fontawesomeIcon", item: "Feature" },
            { icon:"fontawesomeIcon", item: "Feature" }
          ],
          btns: [
            { btntxt: "learn more", url: "https://www.w3schools.com/js/js_json_syntax.asp " },
            { btntxt: "join waitlist", url: " " }
          ]
        },
        {
          sub_header: "dashboard",
          icon: "fontawesomeIcon",
          sub_discription: "BuyChain’s end-to-end platform connects and informs every aspect of your business. The system digitizes your operations, facilitates communication between departments and provides a holistic view of the entire enterprise. ",
          category: "FREE",
          subtittle: "popular features",
          list_items: [
            { icon:"fontawesomeIcon", item: "Feature" },
            { icon:"fontawesomeIcon", item: "Feature" },
            { icon:"fontawesomeIcon", item: "Feature" },
            { icon:"fontawesomeIcon", item: "Feature" }
          ],
          btns: [
            { btntxt: "go to dash board", url: " " }
          ]
        }
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
    alt: ["nogap-bottom", "lavanderbg"],
    embedCode:"",
    shortcode:"",
    content:""
  }

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

      <div v-if="slice.component == 'hero'">
        <hero :herocont="slice.sliceContent" />
      </div>

      <div v-else-if="slice.component == 'split_ImgTxt'">
        <split_ImgTxt :herocont="slice.sliceContent" />
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

      <div :class="container" v-else-if="slice.component == 'newsletter'">
        <newsletter/>
      </div>

    </section>
  </main>

  <!-- ----------------------------- FOOTER ----------------------------- -->

  <footer class="container">
    <footerSlice/>
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
