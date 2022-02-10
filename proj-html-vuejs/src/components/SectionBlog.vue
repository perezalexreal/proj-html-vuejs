<template>
  <div>
    <div class="container-posts">
      <div class="post" v-for="(post,index) in posts" :key="index">
        <div class="poster">
          <div class="details-post">
            <div class="num-post">{{ post.num}}</div>
            <div class="date-post">{{ post.date}}</div>
          </div>
          <img :src="post.urlImage" alt="" />
        </div>
        <p>{{ post.content }}</p>
        <p> <span>by </span>{{ post.author }}</p>
      </div>
    </div>
  </div>
</template>



<script>
export default {
  data(){
    return {
      posts: [
        {
          num: '07',
          date: `May' 19`,
          content: 'This way, loves: a detailed guide through new design',
          urlImage: '/img/h-2-blog-img-1.jpg',
          author: 'Emily Fields',
        },
        {
          num: '07',
          date:`May' 19`,
          content: 'I try to give people a different way of looking art',
          urlImage: '/img/h-2-blog-img-2.jpg',
          author: 'Emily Fields',
        },
        {
          num: '07',
          date:`May' 19`,
          content: 'introduce Richard Laperrière of those amazing features',
          urlImage: '/img/h-2-blog-img-3.jpg',
          author: 'Emily Fields',
        }
      ]
    }
  }
};
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
