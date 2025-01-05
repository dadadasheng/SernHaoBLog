<template>
    <div class="container">
        <div class="navigation_container">
            <h2 @click="router.replace('/')">SernHao.Blog</h2>
            <p class="font-weight-thin" style="font-size: 36px;">
                美食博客
            </p>
        </div>
        <div class="content_container">
            <p v-for="blog in blog_list">
                <span>{{blog}}</span>
            </p>
        </div>
        <div class="content_container">
            <p v-for="blog in blog_list">
                <span>{{blog}}</span>
            </p>
        </div>
        <div id="input_container">
            <v-text-field label="Label" density="compact"></v-text-field>
        </div>
    </div>
</template>

<script setup lang="ts">
  import router from '@/router';
  const blog_list = [
        '极简到建筑的本质',
        '伦敦简单的优雅',
        '极墅之旅&国内高端民宿设计风向',
        '瑞典设计美学风向',
        '极致之墅',
        '简单克制澳洲现代建筑',
        '墨西哥自然的邀约',
        '意大利先锋设计',
        '西雅图住宅风向',
        '极致之墅&中国住宅设计风向',
        '极简到建筑的本质',
        '伦敦简单的优雅',
        '极墅之旅&国内高端民宿设计风向',
        '瑞典设计美学风向',
        '极致之墅',
        '简单克制澳洲现代建筑',
        '墨西哥自然的邀约',
        '意大利先锋设计',
        '西雅图住宅风向',
        '极致之墅&中国住宅设计风向',
        '极简到建筑的本质',
        '伦敦简单的优雅',
        '极墅之旅&国内高端民宿设计风向',
        '瑞典设计美学风向',
        '极致之墅',
        '简单克制澳洲现代建筑',
        '墨西哥自然的邀约',
        '意大利先锋设计',
        '西雅图住宅风向',
        '极致之墅&中国住宅设计风向',
        '极简到建筑的本质',
        '伦敦简单的优雅',
        '极墅之旅&国内高端民宿设计风向',
        '瑞典设计美学风向',
        '极致之墅',
        '简单克制澳洲现代建筑',
        '墨西哥自然的邀约',
        '意大利先锋设计',
        '西雅图住宅风向',
        '极致之墅&中国住宅设计风向'
    ]


</script>

<style scoped>
    .container{
    box-sizing: border-box;
    height: 100%;
    width: 100%;
    padding: 40px;
    display: flex;
    flex-direction: column;
    .navigation_container{
        padding: 20px;
        height: 120px;
        margin-bottom: 20px;
    }
    .content_container{
        display: flex;
        flex-direction: row;
        width: 100%;
        overflow-x: scroll;
        p{
            padding: 0 30px;
            width: 20px;
        }
        span{
            writing-mode: vertical-lr;
            text-orientation: upright;
        }
    }
    .content_container::-webkit-scrollbar{
        display: none;
    }
    }
</style>