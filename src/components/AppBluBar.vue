<script>
export default {
    name: "AppBluBar",
    data(){
      return{
        
        

      }
    }
  }


</script>

<template>
    <div class="container-blu">
        <div class="icon-section">
            <div class="icon-item">
                <img src="../assets/buy-comics-digital-comics.png" alt="">
                <span>DIGITAL COMICS</span>
            </div>
            <div class="icon-item">
                <img src="../assets/buy-comics-merchandise.png" alt="">
                <span>DC MERCHANDISE</span>
            </div>
            <div class="icon-item">
                <img src="../assets/buy-comics-subscriptions.png" alt="">
                <span>SUBSCRIPTION</span>
            </div>
            <div class="icon-item">
                <img src="../assets/buy-comics-shop-locator.png" alt="">
                <span>COMIC SHOP LOCATOR</span>
            </div>
            <div class="icon-item">
                <img src="../assets/buy-dc-power-visa.svg" alt="">
                <span>DC POWER VISA</span>
            </div>
        </div>




    </div>
</template>

<style scoped>
.container-blu {
    padding-left: 17rem;
    padding-right: 17rem;
    background-color: #0282F9;
    height: 6rem;
}

.icon-section {
    
    display: flex;
    justify-content: space-around;
    padding: 20px 0;
    color: #fff;
}


.icon-item {
    display: flex;
    flex-direction: row;
    align-items: center;
    text-align: center;
}

.icon-item img {
    height: 40px;
   padding-right: 1rem;
}

.icon-item span {
    font-size: 12px;
}
</style>