<template>
    <div>
        <div class="header-box">
            <img class="logo-img" :src="logoPath" alt="">
            <div class="container-links">
                <ul v-for="(link,index) in nav" :key="index">
                    <li> {{ link }} </li>
                </ul>
            </div>
        </div>
    </div>
</template>



<script>

export default {
    props: {
        nav: Array,
        logoPath: String
    }
}

</script>


<style lang="scss" scoped>
.logo-img {
    width: 300px;
}
</style>
