<template>
  <div class="home">
      <div>
          <circleLoading></circleLoading>
      </div>
      <div>
          <bubbleLoading></bubbleLoading>
      </div>
  </div>
</template>

<script>
import circleLoading from '../components/circleLoading'
import bubbleLoading from '../components/bubbleLoading'

export default {
    components:{
        circleLoading,
        bubbleLoading
    }
}
</script>

<style>
    .home{
        display: grid;
        grid-template-columns: repeat(2,1fr);
        grid-template-rows: repeat(3,1fr);
        height: 100vh;
        align-items: center;
        justify-items: center;
        max-width: 800px;
        margin: 0 auto;
    }
    .home > div{
        transform: scale(1.5);
    }
</style>