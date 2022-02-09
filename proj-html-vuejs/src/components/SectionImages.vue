<template>
    <div>
        <div class="container-images">
            <img src="../assets/h-2-port-img-1.jpg" alt="">
            <img src="../assets/h-2-port-img-2.jpg" alt="">
            <img src="../assets/h-2-port-img-3.jpg" alt="">
            <img src="../assets/h-2-port-img-4.jpg" alt="">
            <img src="../assets/h-2-port-img-5.jpg" alt="">
            <img src="../assets/h-2-port-img-6.jpg" alt="">
        </div>
    </div>
</template>



<script>
export default {
    
}
</script>


<style lang="scss" scoped>

.container-images {
    display: flex;
    width: 100%;
    flex-wrap: wrap;
    margin: 50px 0px;
    img {
        width: calc(100% / 3);
    }
}

</style>
