<template>
  <div class="container">
    <LargeCardDisplay
      v-for="cardInfo in largeCardSections.slice(0,1)"
      :key="cardInfo.id"
      :cardsSection="cardInfo"
    />
    <SmallCardDisplay
      v-for="cardInfo in smallCardSections"
      :key="cardInfo.id"
      :cardsSection="cardInfo"
    />
  </div>
</template>

<script>
import { largeCardSections, smallCardSections } from '@/assets/data.js'
export default {
  data () {
    return {
      largeCardSections,
      smallCardSections
    }
  }
}
</script>

<style scoped>

</style>
