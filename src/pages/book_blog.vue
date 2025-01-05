<template>
    <div class="container">
        <div class="navigation_container">
            <h2 @click="router.replace('/')">SernHao.Blog</h2>
            <p class="font-weight-thin" style="font-size: 36px;">
                书籍博客
            </p>
        </div>
        <div class="content_container">
            <div class="content_1">
                <div id="book_intro_container">
                    <h1>
                        XXXXXXX 书籍
                    </h1>
                    <p>
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam fuga distinctio tempore aspernatur rem! Optio consequuntur tempore quis, recusandae fuga eaque doloremque consequatur harum velit, dicta, distinctio nesciunt ea officia!
                    </p>
                </div>
                <div id="book_list_container">
                    <p class="list_item" v-for="blog in blog_list">
                        <span>{{blog}}</span>
                    </p>
                </div>
                <div id="input_container">
                    <v-text-field label="Label" density="compact"></v-text-field>
                </div>
            </div>
            <div class="content_2">
                <div id="image_container">

                </div>
            </div>
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
            flex: 1;
            display: flex;
            flex-direction: row;
            width: 100%;
            padding: 10px;
            .content_1{
                flex: 1;
                display: flex;
                flex-direction: column;
                #book_intro_container{
                    height: 150px;
                }
                #book_list_container{
                    flex: 1 1 0;
                    overflow-y: scroll;
                    padding: 10px;
                    .list_item{
                        font-size: 18px;
                        padding: 10px 0;
                    }
                }
                #book_list_container::-webkit-scrollbar{
                    display: none;
                }
                #input_container{
                    height: 80px;
                    padding:  30px 0;
                }
            }
            .content_2{
                height: 100%;
                width: 500px;
                padding: 40px;
                #image_container{
                    height: 100%;
                    width: 100%;
                    
                    background-color: rgb(69, 224, 80);
                }
            }
        }
    }

</style>