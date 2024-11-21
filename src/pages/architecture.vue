<template>
    <div class="container">
        <div class="navigation_container">
            <h2 @click="router.replace('/')">SernHao.Blog</h2>
            <p class="font-weight-thin" style="font-size: 36px;">
                建筑博客
            </p>
        </div>
        <div class="content_container">
            <p class="blog_title">{{ blog_list[current_selected_index] }}</p>
            <v-divider thickness="2" color="#fff" opacity="1"></v-divider>
            <div class="common_container">
                <div class="sub_container">
                    <v-btn width="50" color="#5865f2" style="margin-bottom: 40px; margin-top: 20px;" @click="linkToMagazine()">
                        阅读
                    </v-btn>
                    <div class="catalogue_container">
                        <div class="items_container">
                            <p class="catalogue_item" v-for="(blog_title,index) in blog_list" @click="changeCurrentIndex(index)">{{ blog_title }}</p>
                        </div>
                    </div>
                </div>

                <div class="introduction_container">
                    <div class="img_container">
                        <v-img
                        height="125"
                        src="https://picsum.photos/350/165?random"
                        ></v-img>
                    </div>
                    <div class="introduction_text">
                        {{ introduction_text}}
                    </div>
                </div>
            </div>
        </div>

    </div>
</template>
<script lang="ts" setup>
    import router from '@/router';
    const current_selected_index = ref(0)
    const current_router_index = ref(0)
    const blog_list = [
        '比利时建筑师Nicolas Schuybroek&极简到建筑的本质',
        'Louisa grey&伦敦简单的优雅',
        '极墅之旅&国内高端民宿设计风向',
        'Lotta Agaton&瑞典设计美学风向',
        '极致之墅&Top villas',
        'B.E. Architecture&简单克制澳洲现代建筑',
        'Aagnes Studio&墨西哥自然的邀约',
        'Studiopepe&意大利先锋设计',
        'GoCstudio&西雅图住宅风向',
        '极致之墅&中国住宅设计风向'
    ]
    const introduction_text = ' 地球是我们的家园。地球提供真实的材料、温暖的色彩和归属感。地球是我们需要承担责任的地方。室内设计项目引导我们发现我们与地球的联系，唤起我们的和平感。在这个项目中，大自然激发了我们对色彩和材料的选择，并对设计方法进行了仔细和有意识的思考。自然的色调在一个连贯的物质维度中创造出视觉上的连续性。饰面和家具与室内的陶土、沙土和粘土色调相得益彰。暖色调的灯光、天然和实验性的材料增强了我们与地球的联系感。一个悬浮的大月亮是这个装置的焦点，它重现了置身于宇宙中心的感觉。周围的环境让我们的视觉和触觉都倍感舒适。探索互联智能设备、创新材料及其无限应用的真正感官体验。'
    const changeCurrentIndex = (index)=>{
        console.log('old value:' + current_selected_index.value)
        console.log('new value:' + index)
        current_selected_index.value  = index
        current_router_index.value = index
    }
    const linkToMagazine = ()=>{
        router.replace('magazines/magazine'+(Number(current_router_index.value)+1))
    }
</script>
<style lang="scss" scoped>
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
        padding-bottom: 60px;
        padding-left: 20px;
        padding-right: 20px;
        flex-direction: column;
        .blog_title{
            font-size: 20px;
        }
        .common_container{
            flex: 1;
            display: flex;
            flex-direction: row;
            position: relative;
            .sub_container{
                flex: 1;
                display: flex;
                flex-direction: column;
                .catalogue_container{
                    flex: 1;
                    overflow: auto;
                    position: relative;
                    .items_container{
                        position: absolute;
                        .catalogue_item{
                            font-size: 18px;
                            padding: 10px 0;
                        }
                        .catalogue_item:hover{
                            cursor: pointer;
                        }
                    }
                }
                .catalogue_container::-webkit-scrollbar{
                    display: none;
                }
            
            }
            .introduction_container{
                flex: 1;
                display: flex;
                padding-top: 20px;
                .img_container{
                    width: 250px;
                    height: 180px;
                }
                .introduction_text{
                    flex:1;
                    padding-left: 20px;
                    font-size: 14px;
                    letter-spacing: 2px;
                    color:gray;
                }

            }

        }

    }
    }

</style>