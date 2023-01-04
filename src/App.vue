<script setup>
import NavBar from "./components/NavBar.vue";
import hero from "./components/hero.vue";
import puzzleBreakdown from "./components/puzzleBreakdown.vue";
import getintouch from "./components/getintouch.vue";
import painmap from "./components/painmap.vue";
import newsinsights from "./components/newsinsights.vue";
import newsletter from "./components/newsletter.vue";
import ourprocess from "./components/ourprocess.vue";
import postfeed from "./components/postfeed.vue";
import fetchdata from "./components/fetchdata.vue";
import gBob from "./components/gBob.vue";
import FAQs from "./components/FAQs.vue";
import bob2 from "./components/bob2.vue";
import artcont from "./components/artcont.vue";
import category from "./components/category.vue";
import hero2 from "./components/hero2.vue";

import { ref } from 'vue';

// const quote = ref('')

// axios.get('https://api.kanye.rest/')
//   .then(response => {
//     quote.value = response.data.quote
//     return {
//       quote
//     }
//     console.log(quote);
//   })
// export const useFetch = (url, config = {}) => {
//   const data = ref(null)
//   const response = ref(null)
//   const error = ref(null)
//   const loading = ref(false)

//   const fetch = async () => {
//     loading.value = true
//     try {
//       const result = await axios.request({
//         url,
//         ...config
//       })
//       response.value = result
//       data.value = result.data
//     }
//     catch (ex) {
//       error.value = ex
//     }
//     finally {
//       loading.value = false
//     }
//   }
//   !config.skip && fetch()
//   return { response, error, data, loading, fetch }
// }
// const cacheMap = reactive(new map())
// export const useFetchCache = (key, url, config) => {
//   const update = () => cacheMap.set(key, info.response.value)
//   const clear = () => cacheMap.set(key, undefined)
//   const fetch = async () => {
//     try {
//       await info.fetch()
//       update()
//     }
//     catch {
//       clear()
//     }
//   }
//   const response = computed(() => cacheMap.get(key))
//   const data = computed(() => response.value?.data)
//   if (response.value == null) fetch()
//   return { ...info, fetch, data, response, clear }
// }
const slices = ref([
  {
    bob: "postfeed",
    sliceContent: {
      title: "Nice to Meet You",
      boxcontent: [
        {
          name: "Grace Hancock",
          location: "Los Angeles, CA",
          imageurl: "src/assets/Group 1470.svg",
          para: "This is a very interesting, very succinct bio about what I’ve been doing with my life. I’ll probably share some areas of expertise or maybe a very short fact about my background that’s extremely relevant to GTM since bios are generally very boring. And then maybe close with something douchey like how I graduated summa cum laude.",
          para2: " "
        },
        {
          name: "Grace Hancock",
          location: "Los Angeles, CA",
          imageurl: "src/assets/Group 1470.svg",
          para: "This is a very interesting, very succinct bio about what I’ve been doing with my life. I’ll probably share some areas of expertise or maybe a very short fact about my background that’s extremely relevant to GTM since bios are generally very boring. And then maybe close with something douchey like how I graduated summa cum laude.",
          para2: " "
        },
        {
          name: "Grace Hancock",
          location: "Los Angeles, CA",
          imageurl: "src/assets/Group 1470.svg",
          para: "This is a very interesting, very succinct bio about what I’ve been doing with my life. I’ll probably share some areas of expertise or maybe a very short fact about my background that’s extremely relevant to GTM since bios are generally very boring. And then maybe close with something douchey like how I graduated summa cum laude.",
          para2: " "
        },
        {
          name: "Grace Hancock",
          location: "Los Angeles, CA",
          imageurl: "src/assets/Group 1470.svg",
          para: "This is a very interesting, very succinct bio about what I’ve been doing with my life. I’ll probably share some areas of expertise or maybe a very short fact about my background that’s extremely relevant to GTM since bios are generally very boring. And then maybe close with something douchey like how I graduated summa cum laude.",
          para2: " "
        },
      ]

    }
  },


  {
    bob: "ourprocess",
    sliceContent: {
      title: "Our Process",
      subslice: {
        boxcontent: {
          header: "Phase 1",
          sprintlist: [
            { imageurl: "src/assets/Group 1470.svg", name: "Sprint 1", about: "Established Fact Based", discription: "Collaboratively administrate empowered markets via plug-and-play networks. Dynamically procrastinate B2C users after installed base benefits. Dramatically visualize customer directed convergence without revolutionary ROI."},
            { imageurl: "src/assets/Group 1471.svg", name: "Sprint 2", about: "Strategy Wireframe", discription: "Completely synergize resource taxing relationships via premier niche markets. Professionally cultivate one-to-one customer service with robust ideas. Dynamically innovate resource-leveling customer service for state of the art customer service." },
            { imageurl: "src/assets/Group 1472.svg", name: "Sprint 3", about: "Alignment & Validation", discription: "Objectively innovate empowered manufactured products whereas parallel platforms. Holisticly predominate extensible testing procedures for reliable supply chains. Dramatically engage top-line web services vis-a-vis cutting-edge deliverables." }
          ]
        },
        boxcontent2: {
          header: "Phase 2",
          sprintlist: [
            { imageurl: "src/assets/Puzzle2.svg", header: "Sprint 4", about: "Implimentation & Enablement Sprints", discription: "Objectively innovate empowered manufactured products whereas parallel platforms. Holisticly predominate extensible testing procedures for reliable supply chains. Dramatically engage top-line web services vis-a-vis cutting-edge deliverables." }
          ]
        }
      }, 
    }
  },

  {
    bob: "hero2",
    sliceContent: {
      title: "LBM Operations Software",
      discription: "BuyChain’s end-to-end platform connects and informs every aspect of your business. The system integrates every facet of your operations, facilitating communication between departments and providing a holistic view of the entire enterprise. With real-time inventory management and shipping, AI driven sales order, and financial transparency, you can buy and sell faster, reduce risk and never miss a deal or market move again. ",
      imageurl: "https://placekitten.com/640/360",
      iconurl: [
        { icnurl:"src/assets/btn-xlrg-alt1.svg"},
        { icnurl:"src/assets/btn-xlrg-alt2.svg"},
        { icnurl:"src/assets/btn-xlrg-alt.svg"}
      ]
    }
  },


  {
    bob: "gojo",
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
      details: {
        tittle: "Inventory Management",
        discription: "Our system eliminates time now spent on internal cross-checking by providing all stakeholders real-time inventory data, informing both purchasing and sales on what to buy and what is available to sell. ",
        benlist: [
          {item:"Benifit"},
          {item:"Benifit"},
          {item:"Benifit"},
          {item:"Benifit"},
          {item:"Benifit"},
          {item:"Benifit"},
          {item:"Benifit"},
          {item:"Benifit"},
          {item:"Benifit"},
          {item:"Benifit"},
          
        ]
      }
    }
  },

  {
    bob: "john",
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
    bob: "tommy",
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
        }, {
          date: "01/01/1999",
          articletittle: " article tittle here",
          detail: "BuyChain is the end-to-end supply chain management software for the LBM industry that unifies and mobilizes your team, sales, inventory, and banking in order to meet the demands of an increasingly volatile market.",
          readmore_url: "https://www.w3schools.com/css/css_pseudo_elements.asp"
        }
      ]
    }
  },
  {
    bob: "patrik",
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
    bob: "loki",
    sliceContent: {
      tittle: "Manage Voaltility and Reduce Risk",
      discription: "The BuyChain system eliminates longtime, industry-wide constraints on profitability and growth with the tools, control, and data you need to gain a competitive edge. We have married technology with customer service in a way that has not previously existed in our industry.",
      boxycontent: [
        {
          sub_header: " operations ",
          sub_discription: "BuyChain’s end-to-end platform connects and informs every aspect of your business. The system digitizes your operations, facilitates communication between departments and provides a holistic view of the entire enterprise. ",
          category: " ",
          subtittle: "popular features",
          list_items: [
            { item: "sdfslkdjhf" },
            { item: "sdfslkdjhf" },
            { item: "sdfslkdjhf" },
            { item: "sdfslkdjhf" }
          ],
          btns: [
            { btntxt: "learn more", url: " " },
            { btntxt: "demo", url: " " }
          ]
        },
        {
          sub_header: " capital ",
          sub_discription: "BuyChain’s end-to-end platform connects and informs every aspect of your business. The system digitizes your operations, facilitates communication between departments and provides a holistic view of the entire enterprise. ",
          category: " BETA ",
          subtittle: "popular features",
          list_items: [
            { item: "sdfslkdjhf" },
            { item: "sdfslkdjhf" },
            { item: "sdfslkdjhf" },
            { item: "sdfslkdjhf" }
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
            { item: "sdfslkdjhf" },
            { item: "sdfslkdjhf" },
            { item: "sdfslkdjhf" },
            { item: "sdfslkdjhf" }
          ],
          btns: [
            { btntxt: "go to dash board", url: " " }
          ]
        }
      ]
    }
  },
  {
    bob: "NavBar",
    sliceContent: [
      { label: "Who We Are", url: '' },
      { label: "What We Do", url: '' },
      { label: "News + Insights", url: '' },
      { label: "GTM Pain Map", url: '' },
      { label: "Get In Touch", url: '' }
    ]
  },
  {
    bob: "hero",
    sliceContent: [
      {
        heroImageUrl: '/src/assets/Puzzle.svg',
        label: "Is your GTM Strategy not working?",
        paragraph1: "",
        paragraph2: ""
      }
    ]
  },
  {
    bob: "puzzleBreakdown",
    sliceContent: {
      puzzlePieces: [
        { label: 'GTM Strategy is not well defined', pieceImageUrl: '/src/assets/Path 822.svg' },
        { label: "New process didn't deliver results", pieceImageUrl: '/src/assets/Path 818.svg' },
        { label: "Methodology that isn't being adopted", pieceImageUrl: '/src/assets/Path 821.svg' },
        { label: 'GTM strategy is not performing consistently', pieceImageUrl: '/src/assets/Path 820.svg' },
        { label: "Training but it didn't move the needle", pieceImageUrl: '/src/assets/Path 819.svg' },
        { label: "Methodology didn't produce results", pieceImageUrl: '/src/assets/Path 823.svg' }
      ]
    }
  },
  {
    bob: "hero",
    sliceContent: [
      {
        heroImageUrl: '/src/assets/Puzzle2.svg',
        label: "We can help you put the pieces in place.",
        paragraph1: "Leverage agile frameworks to provide a robust synopsis for high level overviews. Iterative approaches to corporate strategy foster collaborative thinking to further the overall value proposition.Organically grow the holistic world view of disruptive innovation via workplace diversity and empowerment.",
        paragraph2: "Bring to the table win- win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved from generation X is on the runway heading towards a streamlined cloud solution.User generated content in real - time will have multiple touchpoints for offshoring."
      }
    ]
  },
  {
    bob: "getintouch",
    sliceContent: [
      { firstName: " " },
      { lastName: " " },
      { workEmail: " " }
    ]
  },
  {
    bob: "puzzleBreakdown",
    sliceContent: {
      tittle: " What We Do",
      backgroundcolor: "white",
      color: "black",
      puzzlePieces: [
        { label: 'GTM Optimization', pieceImageUrl: '/src/assets/Path 162.svg' },
        { label: "GTM Implentation", pieceImageUrl: '/src/assets/Path 176.svg' },
        { label: "Gong Value Engineering", pieceImageUrl: '/src/assets/Path 180.svg' },
        { label: 'Leadership Coaching', pieceImageUrl: '/src/assets/Path 174.svg' },
        { label: "Skill Field Guides", pieceImageUrl: '/src/assets/Path 170.svg' },
        { label: "Gong Field Guides", pieceImageUrl: '/src/assets/Path 160.svg' }
      ]
    }
  },
  {
    bob: "newsinsights",
    sliceContent: [
      { articleImageUrl: "/src/assets/Puzzle2.svg", label: "News article goes here", date: " 01/01/2023", category: " News + Insights" },
      { articleImageUrl: "/src/assets/Puzzle2.svg", label: "News article goes here", date: " 01/01/2023", category: " News + Insights" },
      { articleImageUrl: "/src/assets/Puzzle2.svg", label: "News article goes here", date: " 01/01/2023", category: " News + Insights" }
    ]
  },

])
</script>

<template>
  <header>
    <div class="wrapper">

      <div v-for="(slice, index) in slices" :key="index">

        <!-- <div v-if="slice.bob == 'hero2'">
          <hero2 :gaara="slice.sliceContent" />
        </div>

        <div v-if="slice.bob == 'gojo'">
          <category :bjon="slice.sliceContent" />
        </div>

        <div v-if="slice.bob == 'john'">
          <artcont :floki="slice.sliceContent" />
        </div>

        <div v-if="slice.bob == 'tommy'">
          <bob2 :ragnar="slice.sliceContent" />
        </div>

        <div v-if="slice.bob == 'patrik'">
          <FAQs :thor="slice.sliceContent" />
        </div>

        <div v-if="slice.bob == 'loki'">
          <gBob :hulk="slice.sliceContent" />
        </div> -->

        <!------------------------------------------------------------------- -->

        <div v-if="slice.bob == 'postfeed'">
          <postfeed :feeds="slice.sliceContent" />
        </div>

        <div v-if="slice.bob == 'ourprocess'">
          <ourprocess :process="slice.sliceContent" />
        </div>

        <div v-if="slice.bob == 'NavBar'">
          <NavBar :navbtn="slice.sliceContent" />
        </div>
        <div v-else-if="slice.bob == 'hero'">
          <hero :herocontent="slice.sliceContent" />
        </div>
        <div v-else-if="slice.bob == 'puzzleBreakdown'">
          <puzzleBreakdown :puzzledata="slice.sliceContent.puzzlePieces" :header="slice.sliceContent.tittle"
            :backgroundcolora="slice.sliceContent.backgroundcolor" />
        </div>
        <div v-else-if="slice.bob == 'getintouch'">
          <getintouch :formcontent="slice.sliceContent" />
        </div>
        <div v-else-if="slice.bob == 'painmap'">
          <painmap />
        </div>
        <div v-else-if="slice.bob == 'newsinsights'">
          <newsinsights :articles="slice.sliceContent" />
        </div>
        <div v-else-if="slice.bob == 'newsletter'">
          <newsletter />
        </div>

      </div>
    </div>
  </header>

  <main>

  </main>
</template>

<style>
@import './assets/main.css'

</style>
