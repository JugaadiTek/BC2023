<script>
const slices = ref([

  {
    component: "hero",
    devnotes: {
      moduleIDs: [01,09,13,25,06,22,31,34,38,40,43],
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
    component: "split_ImgTxt",
    devnotes: {
      moduleIDs: [03,11,14,18,20],
      generalNotes: "",
      moduleSpecificNotes: [
        { id: 0, note: "" }
      ]
    },
    alt: ["nogap-top", "darkbg"],
    sliceContent: {
      brandLogo: [{ url: "url/url", altText: "text" }],
      title: "Made For The Market",
      contentBlocks: [
        {
          discription: "BuyChain is the end-to-end supply chain management software built for the LBM industry. We unify and mobilizes your sales, inventory, and banking so that you can meet the demands of an increasingly volatile market.",
          sub_moduleHotspot: [
            {
              type: "buttons",
              alt: [""],
              buttonlist: [{
                url: "notporn.com",
                text: "sometext",
                type: ["alt1", "class3", "animationX"]
              }]
            },
            {
              type: "iconbutton",
              devnotes: {modules:[3,0], note: "always 3 icon buttons" },
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
              }
            ]
            }
          ]
        }
      ], 
      imageurl: "https://placekitten.com/640/360"
    }
  },
  {
    component: "ctaHero",
    devnotes: {
      moduleIDs: [04,19,28],
      generalNotes: "",
      moduleSpecificNotes: [
        { id: 0, note: "" }
      ]
    }
  },
  {
    component: "hero",
    devnotes: {
      moduleIDs: [0, 0],
      generalNotes: "",
      moduleSpecificNotes: [
        { id: 0, note: "" }
      ]
    },
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
    alt: ["darkbg", "nogap"],
    sliceContent: {
      boxycontent: [
        { item: "Inventory Management", icon: "text"},
      ]
    }
  },

  {
    component: "optionsliceArt",
    alt: ["lightbg"],
    sliceContent: {
      details: {
        tittle: "Inventory Management",
        icon: "text",
        discription: "Our system eliminates time now spent on internal cross-checking by providing all stakeholders real-time inventory data, informing both purchasing and sales on what to buy and what is available to sell. ",
        item_list: [
          [
            { item: "Benifit", icon: "text" },
          ]

        ]
      }
    }
  },

  {
    component: "artcont",
    devnotes: {
      moduleIDs: [0,0],
      generalNotes: "",
      moduleSpecificNotes:[
        {id:0,note:""}
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
    alt: ["lightbg"],
    sliceContent: {
      tittle: "FAQs",
      items_list: [
        { question: "how to sjsdjfosijfooj kjdfglk fdgjl ?", icon: "warehouse", content: "randomtext" },
        { question: "how to sjsdjfosijfooj kjdfglk fdgjl ?", icon: "warehouse", content: "randomtext" }
      ]
    }

  },
  {
    component: "servicecard",
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
          icon: "text",
          sub_discription: "BuyChain’s end-to-end platform connects and informs every aspect of your business. The system digitizes your operations, facilitates communication between departments and provides a holistic view of the entire enterprise. ",
          category: " ",
          subtittle: "popular features",
          list_items: [
            { item: "Feature", icon: "" },
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
          icon: "text",
          sub_discription: "BuyChain’s end-to-end platform connects and informs every aspect of your business. The system digitizes your operations, facilitates communication between departments and provides a holistic view of the entire enterprise. ",
          category: "BETA",
          subtittle: "popular features",
          list_items: [
            { item: "Feature", icon: "" },
          ],
          btns: [
            { btntxt: "learn more", url: "https://www.w3schools.com/js/js_json_syntax.asp " },
            { btntxt: "join waitlist", url: "/url" }
          ]
        },
        {
          sub_header: "dashboard",
          icon: "text",
          sub_discription: "BuyChain’s end-to-end platform connects and informs every aspect of your business. The system digitizes your operations, facilitates communication between departments and provides a holistic view of the entire enterprise. ",
          category: "FREE",
          subtittle: "popular features",
          list_items: [
            { item: "Feature", icon:""},
          ],
          btns: [
            { btntxt: "go to dash board", url: " " }
          ]
        }
      ]
    }
  }

])

</script>



<template>
  <div class="container">
    <div class="inner-container">
      <div class="content">
        <div class="content-block">
          <h1></h1>
          <p></p>
        </div>
      </div>
    </div>

  </div>


</template>

<style scoped>

</style>