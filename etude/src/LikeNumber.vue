<template>
  <div>
  <p>いいね({{ number }})</p>
  <button @click='inclement'>+1</button>
    </div>
</template>

<script>
export default{
  dara() {
    return {
      number:5
    };
  },
  methods:{
      inclement(){
          this.number+=1;
      }
  }
};
</script>
