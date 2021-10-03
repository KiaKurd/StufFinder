<template>
<div>
  <Hero/>
  <LargeCardDisply
  v-for="cardInfo in largeCardInfo"
  :key="cardInfo.id"
  :cardsSetion="cardInfo"
  />
</div>
  
</template>

<script lang="ts">
import { largeCardSections, smallCardSections } from "../assets/data.js"
export default {
  data() {
    return {
      largeCardInfo: largeCardSections,
      smallCardInfo: smallCardSections
    }
  }

}

</script>
