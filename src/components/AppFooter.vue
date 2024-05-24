<script>
export default {
    name: "AppFooter",
    data() {

        return {
            menus: [
                {
                    title: 'DC COMICS',
                    links: [
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Videos',
                        'News',
                    ],

                },
                {
                    title: 'SHOP',
                    links: [
                        'Shop DC',
                        'Shop DC Collectibles',
                    ],
                },
                {
                    title: 'DC',
                    links: [
                        'Terms Of Use',
                        'Privacy policy (New)',
                        'Ad Choices',
                        'Advertising',
                        'Jobs',
                        'Subscriptions',
                        'Talent Workshops',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop Help',
                        'Contact Us',
                    ],
                },
                {
                    title: 'SITES',
                    links: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa',
                    ],
                },
            ],
        };
    }
}
</script>
<!---------------------------------- HTML ---------------------------------->
<template>
    <div class="container-footer">
        
        <!-- link footer -->
        <div class="col-link">

            <div v-for="(menu, index) in menus" :key="index" class="menu">
                <h2>{{ menu.title }}</h2>
                <ul>
                    <li v-for="(link, linkIndex) in menu.links" :key="linkIndex">{{ link }}</li>
                </ul>
            </div>

        </div>
        <!-- immagine laterale -->
        <div class="col-img">
            <img src="../assets/dc-logo-bg.png" alt="">
        </div>
        <!-- sign up -->
    </div>
    <div class="under-footer">
        <div class="sign-up">
            <button class="sign-button">SIGN-UP NOW!</button>
        </div>
        <div class="social">
            <span class="follow-us">FOLLOW US</span>
            <div class="icons">
                <ul class="row social-list">
              <li class="social-item">
                <img src="../assets/footer-facebook.png" alt="">
              </li>
              <li class="social-item">
                <img src="../assets/footer-twitter.png" alt="">
              </li>
              <li class="social-item">
                <img src="../assets/footer-youtube.png" alt="">
              </li>
              <li class="social-item">
                <img src="../assets/footer-pinterest.png" alt="">
              </li>
              <li class="social-item">
                <img src="../assets/footer-periscope.png" alt="">
              </li>
            </ul>
            </div>
        </div>
    </div>

</template>
<!-------------------------------- CSS ---------------------------->
<style scoped>
.container-footer {
    display: flex;
    flex-direction: row;
    background-image: url(../assets/footer-bg.jpg);
    height: 50vh;
    object-fit: cover;
}

/* colonna di sinstra con i link */
.col-link {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding-left: 17rem;
    padding-top: 2rem;
    color: rgb(190, 190, 190);
    width: 50%;
}

.menu {
    flex: 1;
    margin: 0 10px;
}

.menu h2 {
    color: white;
    font-size: 1.2em;
    margin-bottom: 10px;
}

.menu ul {
    list-style-type: none;
    font-size: 0.8em;

}

.menu li {
    margin-bottom: 5px;
}

/* colonna di destra con immagine  */
.col-img {
    width: 50%;
    height: 100%;
    overflow: hidden;
}

.col-img img {
    width: 70%;
    height: 100%;
    object-fit: cover;
}

/* riga sign up */
.under-footer {
    display: flex;
    flex-direction: row;
    padding-left: 17rem;
    padding-right: 17rem;
    align-items: center;
    height: 6rem;
    background-color: #303030;
    justify-content: space-between;
}

.sign-button {
    border: solid #1d77ff;
    padding: 10px 20px;
    background-color: #303030;
    color: white;
    font-weight: bold
}
.social{
    display: flex;
    flex-direction: row;
}
.sign-up {
    align-content: center;
}

.social-list {
    gap: 1rem;
    list-style-type: none;
    display: flex;
    flex-direction: row;
    align-items: center;
}

.follow-us {
    padding-top: 0.6rem;
    padding-right: 1rem;
    margin-right: 10px;
    color: #1d77ff;
    font-weight: bold
}
</style>