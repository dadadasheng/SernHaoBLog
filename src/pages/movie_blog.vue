<template>
    <div class="container">
        <div class="navigation_container">
            <h2 @click="router.replace('/')">SernHao.Blog</h2>
            <p class="font-weight-thin" style="font-size: 36px;">
                电影博客
            </p>
        </div>
        <div class="content_container">
            <div class="right_container">
                <div class="blog_title">
                    <p>
                        《盗梦空间》中的梦境与现实
                    </p>
                </div>
                <div class="blog_list">
                    <p class="list_item" v-for="blog in blog_list">
                        {{ blog }}
                    </p>
                </div>
                <div id="input_container">
                        <v-text-field label="Label" density="compact"></v-text-field>
                </div>
            </div>
            <div class="left_container">
                <div class="text_intro_container">
                    {{introduction_text}}
                </div>
                <div class="other_intro_container">
                    
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
    const introduction_text = ' 地球是我们的家园。地球提供真实的材料、温暖的色彩和归属感。地球是我们需要承担责任的地方。室内设计项目引导我们发现我们与地球的联系，唤起我们的和平感。'
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
        .content_container{
            flex: 1;
            display: flex;
            flex-direction: row;
            .right_container{
                flex: 1;
                display: flex;
                flex-direction: column;
                .blog_title{
                    height: 100px;
                    border-style: solid;
                    border-width: 0 0 1px 0;
                    padding: 30px 0;
                    font-size: 32px;
                    font-weight: lighter;
                }
                .blog_list{
                    flex: 1 0 0;
                    padding-top: 20px;
                    overflow: auto;
                    .list_item{
                        font-size: 18px;
                        padding: 10px 0;
                    }
                }
                .blog_list::-webkit-scrollbar{
                    display: none;
                }
                #input_container{
                    height: fit-content;
                    padding-right: 50px;
                    margin-top: 10px;

                }
            }
            .left_container{
                width: 400px;
                display: flex;
                flex-direction: column;
                .text_intro_container{
                    height: 100px;
                    border-style: solid;
                    border-width: 0 0 1px 1px;
                    font-size: 14px;
                    padding: 10px;
                }
                .other_intro_container{
                    flex: 1;
                    border-style: solid;
                    border-width: 0 0 0 1px;
                    margin-bottom: 20px;
                }
            }
        }
    }
</style>