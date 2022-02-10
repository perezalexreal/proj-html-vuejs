<template>
  <div>
    <div class="container-box">
      <div class="arrow-slider">
        <img @click="previewContent" src="../assets/arrow-left.png" alt="" />
      </div>
      <div class="left-box">
        <h1>
          {{ sliderContent[currentIndex].title }}
          <span> {{ sliderContent[currentIndex].italic }} </span>
        </h1>
        <p class="txt-color">
          {{ sliderContent[currentIndex].content }}
        </p>
        <a href="#">
          <button class="btn-cta brd-beige btn-txt">Read More</button></a
        >
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
        <img @click="nextContent" src="../assets/arrow-right.png" alt="" />
      </div>
    </div>
    <div class="container-dots">
    <div
      :class="['dots-container', currentIndex]"
      v-for="(dots, i) in sliderContent"
      :key="i"
    >
      <div :class="['dots', currentIndex == i ? 'current-dot' : '']"></div>
    </div>

    </div>

    <div></div>
  </div>
</template>



<script>
export default {
  data() {
    return {
      currentIndex: 0,
      sliderContent: [
        {
          title: "Devotion that never",
          italic: "ends",
          content:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Beatae eos in optio excepturi natus illo ipsa dolor id aliquam quaerat!",
        },
        {
          title: "Another Title that never",
          italic: "ends",
          content:
            "Incidunt qui quo porro error pariatur alias, debitis at. Sequi, quasi!",
        },
        {
          title: "Second best ever title in the",
          italic: "world",
          content:
            "Ipsum dolor sit amet, consectetur adipisicing elit. Eaque excepturi odit eos blanditiis libero iusto ea quis autem dignissimos ",
        },
      ],
    };
  },
  methods: {
    nextContent: function () {
      if (this.currentIndex === this.sliderContent.length - 1) {
        this.currentIndex = 0;
      } else {
        this.currentIndex++;
      }
      // todo -> e se arrivo alla fine dell'array?
    },
    previewContent: function () {
      if (this.currentIndex === 0) {
        this.currentIndex = this.sliderContent.length - 1;
      } else {
        this.currentIndex--;
      }
      // todo -> e se arrivo a 0?
    },
  },
};
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
}

.dots {
  width: 10px;
  height: 10px;
  background: $brd-beige;
  margin: 0px 3px;
  border-radius: 50px;
  cursor: pointer;
}

.current-dot {
  width: 15px;
  height: 15px;
}

.container-dots {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
