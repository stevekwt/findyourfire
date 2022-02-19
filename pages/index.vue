<template>
    <div class="">
      <div class="container">
        <Hero />
        <LargeCardDisplay
          v-for="cardInfo in largeCardInfo"
          :key="cardInfo.id"
          :cardsSection="cardInfo" 
        />
        <SmallCardDisplay
          v-for="cardInfo in smallCardInfo"
          :key="cardInfo.id"
          :cardsSection="cardInfo" 
        />
      </div>
    </div>
</template>

<script>
// import LargeCardDisplay from "../components/LargeCardDisplay.vue";
import { largeCardSections, smallCardSections } from "@/assets/data.js"
export default {
  data() {
    return {
      largeCardInfo: largeCardSections,
      smallCardInfo: smallCardSections
    }
  }
    // name: "IndexPage",
    // head: {
    //     title: "Fiery Foundlings Fight Fire With Fire",
    //     meta: [
    //         {
    //             hid: "description",
    //             name: "description",
    //             content: "Fiery foundlings will find your fire fighting and fight fire with fire"
    //         }
    //     ]
    // }
    // // metaInfo: {
    // //   title: 'Default Title for Fire Finding',
    // //   titleTemplate: '%s | Fire Finding'
    // // }
    // ,
    // components: { LargeCardDisplay }
}
</script>
