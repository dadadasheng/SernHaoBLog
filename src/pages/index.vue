<template>
  <div class="container"> 
      <div class="websiteTitleContainer">
        <div class="websiteTitle">
          SernHao.BLog
        </div>
        <div class="navigation">
          <v-container>
            <v-row>
              <v-col class="cursor-pointer link" v-for="item in navigation_items" @click="router.replace(item.path)">
                <span>
                  {{ item.title }}
                </span>
              </v-col>
            </v-row>
          </v-container>
        </div>
      </div>
  </div>

</template>

<script lang="ts" setup>
  import router from '@/router';
  // navigation
  const navigation_items = [
    {
      title:'建筑博客',
      path:'/architecture'
    },
    {
      title:'电影博客',
      path:'/movie_blog'
    },
    {
      title:'音乐博客',
      path:'/music_blog'
    },
    {
      title:'美食博客',
      path:'/food_blog'
    },
    {
      title:'书籍博客',
      path:'/book_blog'
    },
    {
      title:'更多主题',
      path:'/'
    },
    {
      title:'关于作者',
      path:'/'
    }
  ]
  
</script>

<style lang="scss" scoped>
.container{
  position: relative;
  height: 100%;
  width: 100%;
  .websiteTitleContainer{
    position: absolute;
    top: 50%;
    right: 50%;
    transform: translateY(-50%) translateX(50%);
    
    .websiteTitle{
      text-align: center;
      font-size: 64px;
    }
    .navigation{
      display: flex;
      p{
        padding: 20px;

      }
      .link{
          color: #8b8b8b;
      }
      .link:hover{
          color: #fff;
      }
    }
  }
}
// :global(html::-webkit-scrollbar){
//   display: none;
// }
</style>