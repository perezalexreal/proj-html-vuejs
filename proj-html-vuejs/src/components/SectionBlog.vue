<template>
  <div>
    <div class="container-posts">
      <div class="post">
        <div class="poster">
          <div class="details-post">
            <div class="num-post">07</div>
            <div class="date-post">May 18</div>
          </div>
          <img src="../assets/h-2-blog-img-1.jpg" alt="" />
        </div>
        <p>This way, loves: a detailed guide through new design</p>
        <p>By Emily Fields</p>
      </div>
      <div class="post">
        <div class="poster">
          <div class="details-post">
            <div class="num-post">07</div>
            <div class="date-post">May 18</div>
          </div>
          <img src="../assets/h-2-blog-img-1.jpg" alt="" />
        </div>
        <p>This way, loves: a detailed guide through new design</p>
        <p>By Emily Fields</p>
      </div>
      <div class="post">
        <div class="poster">
          <div class="details-post">
            <div class="num-post">07</div>
            <div class="date-post">May 18</div>
          </div>
          <img src="../assets/h-2-blog-img-1.jpg" alt="" />
        </div>
        <p>This way, loves: a detailed guide through new design</p>
        <p>By Emily Fields</p>
      </div>
    </div>
  </div>
</template>



<script>
export default {};
</script>


<style lang="scss" scoped>
@import "./style/main.scss";

.container-posts {
  display: flex;
  width: 100%;
  padding: 80px 100px;

  .post {
    width: calc(100% / 3);
    margin: 30px 20px;

    .poster {
      img {
        width: 100%;
      }

      .details-post {
        position: relative;
        left: 15px;
        top: 55px;
        width: 60px;

        .num-post {
          background: $green;
          height: 40px;
          text-align: center;
          font-weight: 800;
          font-size: 26px;
          font-style: italic;
        }
        .date-post {
          background: $rose;
          height: 40px;
          font-size: 12px;
          font-weight: 500;
          text-align: center;
          text-transform: uppercase;
          vertical-align: middle;
          line-height: 35px;
          clip-path: polygon(0% 0%, 100% 0%, 100% 100%, 50% 81%, 0 100%);
        }
      }
    }
  }
}
</style>
