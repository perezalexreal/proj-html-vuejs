<template>
    <div class="footer-box">
        <div class="box">
            <img src="../assets/logo-sidearea-1.png" alt="">
            <p> Let's Get Creative</p>
        </div>
        <div class="box">
            <p> maree.qode@gmail.com</p>
            <p>+44645 321 789</p>
        </div>
        <div class="box">
            <p>Avenue d'Auderghem 10</p>
            <p>1040 Brusels, Belgium</p>
        </div>
        <div class="box">
            <p>Stai in touch with us</p>
            <div class="social-links" v-for="(social,index) in socials" :key="index">
               <a :href="social.urlLogo"><img :src="social.urlImage" alt=""></a> 
            </div>
        </div>
    </div>
</template>



<script>
export default {
    data () {
        return {
            socials: [
                {
                    urlImage: '/img/socials/twitter.png',
                    urlLogo: 'https://www.twitter.com'
                },
                {
                    urlImage: '/img/socials/pinterest.png',
                    urlLogo: 'https://www.pinterest.com'
                },
                {
                    urlImage: '/img/socials/facebook-app-symbol.png',
                    urlLogo: 'https://www.facebook.com'
                },
                {
                    urlImage: '/img/socials/linkedin.png',
                    urlLogo: 'https://www.linkedin.com'
                },
            ]
        }
    }
}
</script>


<style lang="scss" scoped>
@import "./style/main.scss";

.footer-box {
    display: flex;
    padding: 70px 120px;
    justify-content: center;
    width: 100%;
    background: $light-green;

    .box {
        width: calc(100% / 4);
        text-align: left;
    }
}

.social-links {
    display: inline;
    width: auto;
    margin: 0px 10px;
    padding: 10px 0px;
    img {
        margin-top: 10px;
        width: 20px;
    }
}

</style>
