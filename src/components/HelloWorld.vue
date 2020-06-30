<template>
  <div class="hello">
    <h1>bye bye</h1>

  </div>
</template>
<script>
import { TimelineLite } from 'gsap'

export default {
  mounted () {
    const timeline = new TimelineLite()
    this.$nextTick(function () {
      timeline.to('h1', 5, {x: 100})
    })
  }
}
</script>

<style  scoped>
 h1{
   color: blue;
 }
</style>
