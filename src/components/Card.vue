<script>
export default {
name:"Card",

props: {
      series: String,
      thumb: String,
    }


}
</script>

<template>
    <li class="card">
    <div class="comic-image">
      <img class="comic-image" :src="thumb" alt="">
    </div>
    <h3 class="card-title">{{ series }}</h3>
  </li>

</template>

<style scoped>
.card{
    list-style: none;
    padding: 15px;
  }

  .comic-image{
    object-fit: contain;
    object-position: top;
    width: 140px;
    height: 150px;
  }

 

</style>