<script>
export default {
    data(){
      return{
        
        menuItems: [

          {
            itemClass: 'menu-item',
            itemSpec: 'CHARACTER',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'COMICS',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'MOVIES',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'TV',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'GAMES',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'COLLECTIBLES',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'VIDEOS',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'FANS',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'NEWS',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'SHOP',
          },

        ]


      }
    }
  }
</script>

<template>
  <header>
    <div class="container header">
        <div class="logo">
            <img src="../assets/dc-logo.png" alt="">
        </div>
        
            <ul class="menu">
            <li v-for="(el,i) in menuItems" class="menu-item">{{ menuItems[i].itemSpec }}</li>
          </ul>
       
      
    </div>
    </header>
</template>

<style scoped>
.container{
    padding: 0 15rem;
    display: flex;
    flex-direction: row;
    height: 20vh;
}
    
.header{
    justify-content: space-between;
}

.menu{
    align-items: center;
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 15px;
    list-style: none;
    
}

.menu-item{
    color: rgb(110, 109, 109);
    font-weight: 600;
}
.logo{
    margin: 0.5rem;
}

</style>