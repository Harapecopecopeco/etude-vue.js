<template>
  <div>
    <p>いいね({{ halfNumber }})</p>
    <button @click="increment">+1</button>
   </div>
</template>

<script>
export default{
  props:{
    totalNumber: {
      type: Number,
      required: true  
    }
  },
  computed:{
    halfNumber(){
      return this.halfNumber /2
    }
  },
  methods:{
      increment() {
          this.number+=1;
      }
  }
};
</script>

<style scoped>
  div {
    border: 1px solid red;
  }
</style>