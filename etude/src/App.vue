<template>
  <div>
  <LikeHeader></LikeHeader>
  <p>{{ number/2 }}</p>
  <LikeNumber :totalNumber="6"></LikeNumber>
  <LikeNumber :total-number="6"></LikeNumber>
  </div>
</template>

<script>
import LikeHeader from './components/LikeHeader.vue';

export default{
  data(){
    return {
      number:10
    };
  },
  components:{
    LikeHeader
  }
};
</script>

<style scoped>
  div {
    border: 1px solid blue;
  }
</style>