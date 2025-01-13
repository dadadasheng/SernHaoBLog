<template>
    <div class="container">
        <div class="navigation_container">
            <h2 @click="router.replace('/')">SernHao.Blog</h2>
            <p class="font-weight-thin" style="font-size: 36px;">
                美食博客
            </p>
        </div>
        <div class="intro_container" v-if="false">
            <div class="title_container">
                <p>
                    极简到建筑的本质
                </p>
            </div>
            <div class="introduction_container">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nobis, odit atque quod modi possimus minus pariatur id iure alias molestias debitis saepe doloribus voluptatum. Quae repellendus quam voluptatibus ipsa commodi.</div>
            <div class="image_container">
                <v-img
                        :aspect-ratio="1"
                        class="bg-white"
                        src="https://cdn.vuetifyjs.com/images/parallax/material.jpg"
                        height="100%"
                        cover
                    ></v-img>
            </div>
            <div class="button_container">
                <p>
                    阅读
                </p>
            </div>
        </div>
        <div class="content_container">
            <p v-for="blog in blog_list">
                <span>{{blog}}</span>
            </p>
        </div>
        <div id="input_container">
            <v-text-field label="Label" density="compact"  variant="underlined"></v-text-field>
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
        }
        .intro_container{
            height: 150px;
            border-style: solid;
            border-width: 0 0 1px 0;
            margin-bottom: 10px;
            display: flex;
            flex-direction: row;
            width: 100%;
            .title_container{
                width: 40px;
                p{
                    writing-mode: vertical-lr;
                    text-orientation: upright;
                }
            }
            .introduction_container{
                flex: 3;
            }
            .image_container{
                flex: 1;
            }
            .button_container{
                width: 50px;
                p{
                    writing-mode: vertical-lr;
                    text-orientation: upright;
                }
            }
        }
        .content_container{
            flex: 1;
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