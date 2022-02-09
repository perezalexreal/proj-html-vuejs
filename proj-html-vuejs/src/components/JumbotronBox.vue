<template>
  <div>
    <div class="container-box">
        <div class="arrow-slider">
           <img src="../assets/arrow-left.png" alt="">
          
        </div>
      <div class="left-box">
        <h1>Devotion that never <span> ends</span></h1>
        <p class="txt-color">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Beatae eos in
          optio excepturi natus illo ipsa dolor id aliquam quaerat!
        </p>
        <a href="#"> <button class="btn-cta brd-beige btn-txt">Read More</button></a>
      </div>
      <div class="right-box">
        <div class="svgs">
          <img
            class="hero-img"
            src="../assets/short-slider-rev-1-img-2.png"
            alt=""
          />
          <img class="hero-img" src="../assets/h-2-slider-img-12.png" alt="" />
          <img class="hero-img" src="../assets/h-2-slider-img-13.png" alt="" />
        </div>
        <img class="hero-img" src="../assets/h-2-slider-img-15.png" alt="" />
        <img class="hero-img" src="../assets/h-2-slider-img-16.png" alt="" />
        <div class="svgs">
          <img class="hero-img" src="../assets/h-2-slider-img-14.png" alt="" />
          <img
            class="hero-img"
            src="../assets/short-slider-rev-1-img-6.png"
            alt=""
          />
          <img class="hero-img" src="../assets/h-2-slider-img-17.png" alt="" />
        </div>
      </div>
              <div class="arrow-slider">
            <img src="../assets/arrow-right.png" alt="">
        </div>
    </div>
    <div class="dots-container">
        <div class="dots"></div>
        <div class="dots"></div>
        <div class="dots"></div>
    </div>
  </div>
</template>



<script>
export default {};
</script>


<style lang="scss" scoped>
@import "./style/main.scss";

.container-box {
  display: flex;
  justify-content: space-between;
  padding: 50px 0px;
  max-height: 400px;
  height: 100%;

  .left-box {
      width: 60%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding-left: 20px;

    h1 {
      font-size: 70px;
      white-space: 2px;
      font-weight: 300;
      line-height: 1em;


      span {
        font-weight: 800;
        font-style: italic;
      }
    }

    p {
      width: 70%;
    }
  }
  .right-box {
      display: flex;
      width: 40%;
      text-align: left;
  }
}

.svgs {
    display: flex;
    justify-content: space-between;
    flex-direction: column;

    img {
        width: 40px;
    }
}

.arrow-slider {
    margin: 0px 40px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 25px;
    
    img {
         cursor: pointer;
    }
}

.dots-container {
    display: flex;
    justify-content: center;
    .dots {
        width: 10px;
        height: 10px;
        background: $brd-beige;
        margin: 0px 8px;
        border-radius: 50px;
        cursor: pointer
    }
}
</style>
