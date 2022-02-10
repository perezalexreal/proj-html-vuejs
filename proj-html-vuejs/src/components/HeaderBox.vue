<template>
    <div>
        <div class="header-box">
            <img class="logo-img" src="../assets/logo-sidearea-1.png" alt="">
            <div class="menu-right">
            <div class="container-links">
                <ul v-for="(link,index) in nav" :key="index">
                    <li> {{ link }} </li>
                </ul>
            </div>
            <img class="menu-mobile-logo" src="../assets/svg/svg-1.svg" alt="">
            </div>
        </div>
    </div>
</template>



<script>

export default {
    props: {
        nav: Array,
    }
}

</script>


<style lang="scss" scoped>


.header-box {
    height: 80px;
    background-color: white;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0px 30px;

    .menu-right {
        display: flex;
    }

    .container-links {
        display: flex;

        ul li {
            list-style: none;
            margin: 0px 15px;
            cursor: pointer;
            border: 1px solid transparent;
            text-transform: uppercase;
            font-size: 13px;
            letter-spacing: 2px;
            font-weight: 500;

            &:hover {
                border-bottom: 2px solid #f5d8ca;
            }
      }
    }

    .menu-mobile-logo{
        width: auto;
        height: 20px;
        margin-left: 15px;
        cursor: pointer;
    }
}


.logo-img {
    width: auto;
    max-height: 30px;
}
</style>
