<template>
  <div>
    <button @click="addlike">like</button>
    <button @click="adddislike">dislike</button>
    <div>
      Колличество лайков <strong>{{ likes }}</strong>
    </div>
    <div>
      Колличество дизлайков <strong>{{ dislikes }}</strong>
    </div>

    
  </div>
</template>
<script>
  export default{
    data(){
      return{
        likes:0,
        dislikes:0,
      }
    },
    methods:{
      addlike(){
        this.likes +=1;
      },
      adddislike(){
        this.dislikes +=1;
      }
    }
  }

</script>
<style>


</style>
