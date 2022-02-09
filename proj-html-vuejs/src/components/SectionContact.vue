<template>
    <div>
        <div class="container-box">
            <h1> Want to work with us? Send us <span> a message</span> </h1>
            <p class="txt-color"> Lorem, ipsum dolor sit amet consectetur adipisicing elit. Veritatis odio dolore consequatur ullam dolorum, nihil totam consectetur omnis nostrum mollitia magni nobis ea porro perferendis rerum tempora culpa ab fuga?</p>
            <a href=""> <button class="btn-cta btn-txt brd-lightgreen"> Contact</button></a>
        </div>
    </div>
</template>



<script>
export default {
    
}
</script>


<style lang="scss" scoped>

@import "./style/main.scss";

.container-box {
    background-image: url('../assets/h-2-background-1.jpg') ;
    background-size: cover;
    background-repeat: no-repeat;
    height: 400px;
    text-align: center;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    padding: 0px 100px;
    
    h1 {
        font-size: 40px;
        font-weight: 400;
        span {
            font-style: italic;
            font-weight: 800;
        }
    }
    p {
        margin: 25px 0px;
    }
}

</style>
