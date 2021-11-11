<template>
  <div>
    <Hero />
    <LargeCardDisplay
      v-for="cardInfo in largeCardInfo"
      :key="cardInfo.id"
      :cards-section="cardInfo"
    />
    <SmallCardDisplay
      v-for="cardInfo in smallCardSections"
      :key="cardInfo.id"
      :cards-section="cardInfo"
    />
  </div>
</template>

<script>
// import Hero from '../components/Hero.vue'
// import LargeCardDisplay from '../components/LargeCardDisplay.vue'
// import SmallCardDisplay from '../components/SmallCardDisplay.vue'
import { largeCardSections, smallCardSections } from '@/assets/data.js'
export default {
  // components: {
  //   Hero,
  //   LargeCardDisplay
  // },
  data () {
    return {
      largeCardInfo: largeCardSections,
      smallCardSections
    }
  }
}
</script>
