<template>
    <div class="container">
        <div class="navigation_container">
            <h2 @click="router.replace('/')">SernHao.Blog</h2>
            <p class="font-weight-thin" style="font-size: 36px;">
                音乐博客
            </p>
        </div>
        <div class="content_container">
            <div class="blog_title">
                <h2>
                    《盗梦空间》中的梦境与现实
                </h2>
            </div>
            <div class="list_container">
                <div class="blog_image">

                </div>
                <div class="blog_list">
                    <div class="list">
                    <p class="list_item" v-for="blog in blog_list">
                        {{ blog }}
                    </p>
                    </div>

                </div>
                <div class="blog_intro_container">
                    {{introduction_text}}
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
    const introduction_text = ' 地球是我们的家园。地球提供真实的材料、温暖的色彩和归属感。地球是我们需要承担责任的地方。室内设计项目引导我们发现我们与地球的联系，唤起我们的和平感。在这个项目中，大自然激发了我们对色彩和材料的选择，并对设计方法进行了仔细和有意识的思考。自然的色调在一个连贯的物质维度中创造出视觉上的连续性。饰面和家具与室内的陶土、沙土和粘土色调相得益彰。暖色调的灯光、天然和实验性的材料增强了我们与地球的联系感。一个悬浮的大月亮是这个装置的焦点，它重现了置身于宇宙中心的感觉。周围的环境让我们的视觉和触觉都倍感舒适。探索互联智能设备、创新材料及其无限应用的真正感官体验。'
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
            flex: 1 0 0;
            display: flex;
            flex-direction: column;
            .blog_title{
                position: relative;
                padding-bottom: 10px;
                margin-bottom: 20px;
                border-style: solid;
                border-width: 0 0 1px 0;
                text-align: center;
                height: 50px;
            }
            .list_container{
                flex: 1 0 0;
                display: flex;
                .blog_image{
                    width: 300px;
                    background-color: antiquewhite;
                    border-radius: 20px;
                }
                .blog_intro_container{
                    width: 300px;
                }
                .blog_list{
                    flex: 1 0 0;
                    text-align: center;
                    padding-left: 24px;
                    overflow: auto;
                    display: flex;
                    flex-direction: column;
                    .list{
                        flex: 1 0 0;
                        overflow: auto;
                        .list_item{
                            font-size: 18px;
                            padding: 10px 0;
                        }
                    }
                    .list::-webkit-scrollbar{
                        display: none;
                    }
                }

            }
        }

    }
</style>