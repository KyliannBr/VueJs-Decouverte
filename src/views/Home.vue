<template>
  <div class="home">
    <HalfPage path="M18.31 8.22H0M11.16 1l7.15 7.15-7.33 7.34" />
    <BigText />
  </div>
</template>

<script>
// @ is an alias to /src
import HalfPage from '@/components/HalfPage.vue'
import BigText from '@/components/BigText.vue'

export default {
  name: 'Home',
  components: {
    HalfPage, BigText
  }
}
</script>
