<template>
    <div>
        <div class="container-images">
            <img class="img" src="../assets/h-2-port-img-1.jpg" alt="">
            <img class="img" src="../assets/h-2-port-img-2.jpg" alt="">
            <img class="img" src="../assets/h-2-port-img-3.jpg" alt="">
                 <img  class="float-img-first" src="/img/svg/svg-4.svg" alt="">
                 <img  class="float-img-second" src="/img/svg/svg-6.svg" alt="">
            <img  class="img" src="../assets/h-2-port-img-4.jpg" alt="">
            <img class="img" src="../assets/h-2-port-img-5.jpg" alt="">
            <img class="img" src="../assets/h-2-port-img-6.jpg" alt="">
               <img  class="float-img-third" src="/img/svg/svg-2.svg" alt="">
                 <img  class="float-img-four" src="/img/svg/svg-2.svg" alt="">
        </div>
        <div class="contain-fl-images">
       
        </div>
    </div>
</template>



<script>
export default {
    
}
</script>


<style lang="scss" scoped>
@import "./style/main.scss";

.container-images {
    display: flex;
    width: 100%;
    flex-wrap: wrap;
    margin: 50px 0px;
    .img {
        width: calc(100% / 3);
    }
}

.contain-fl-images {
    position: absolute
}

.float-img-first {
    width: 40px;
    padding: 10px;
    background: #ee2852;
    position: absolute;
    right: 0;
    bottom: 45px;
}

.float-img-second {
    width: 40px;
    padding: 10px;
    background: white;
    position: absolute;
    right: 0;
    bottom: 0px;
}

.float-img-third {
    width: 30px;
    padding: 10px;
    background: $light-green;
    position: absolute;
    right: 0;
    bottom: -865px
}

.float-img-four {
    width: 30px;
    padding: 10px;
    background: $light-green;
    position: absolute;
    right: 0;
    bottom: -415px
}
</style>
