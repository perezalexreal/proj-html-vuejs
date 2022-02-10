<template>
    <div>
        <div class="container-box">
            <h1> Working <span> process</span> </h1>
            <div class="box-features">
                <div class="features">
                    <img  src="/img/work/1.png"  alt="">
                    <h1> First theres an idea</h1>
                    <p> Lorem ipsum dolor sit amet consectetur adipisicing elit. Error, deserunt molestiae!</p>
                </div>
                <div class="features">
                    <img  src="/img/work/2.png"  alt="">
                    <h1> Then we talk about</h1>
                    <p> Lorem ipsum dolor sit amet consectetur adipisicing elit. Error, deserunt molestiae!</p>
                </div>
                <div class="features">
                    <img  src="/img/work/3.png"  alt="">
                    <h1> And we think about</h1>
                    <p> Lorem ipsum dolor sit amet consectetur adipisicing elit. Error, deserunt molestiae!</p>
                </div>
                <div class="features">
                    <img src="/img/work/4.png" alt="">
                    <h1> So we draw along</h1>
                    <p> Lorem ipsum dolor sit amet consectetur adipisicing elit. Error, deserunt molestiae!</p>
                </div>
            </div>
        </div>
    </div>
</template>



<script>
export default {
    
}
</script>


<style lang="scss" scoped>

.container-box {
    text-align: center;
    padding: 60px 100px;
    background: url('../assets/svg/svg-3.svg') no-repeat center;

    h1 {
        font-size: 40px;
        font-weight: 400;
        margin-bottom: 30px;
         span {
             font-style: italic;
             font-weight: 800;
         }
    }
    .box-features{
        display: flex;
        margin-bottom: 30px;
        

        .features {
            padding: 20px 30px;


            h1 {
                font-size: 25px;
            }

            p {
                font-size: 14px;
            }

            img {
                background: #faf7f1;
                width: 175px;
                height: 175px;
                border-radius: 100px;
                padding: 65px;
            }
        }
    }
}

</style>
