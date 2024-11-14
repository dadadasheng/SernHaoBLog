<template>
    <div class="container">
        <div class="navigation_container">
            <h2>SernHao.Blog</h2>
            <p class="font-weight-light" style="font-size: 36px;">
                建筑博客
            </p>
        </div>
        <div class="catalogue_container">
            <div v-for="(blog_item,index) in blog_list" key="index"  class="catalogue_item" @click="changeCurrentIndex(index)">
                <p  style="padding: 10px 0px; font-size: 18px;" >
                    {{ blog_item }}
                </p>   
                <v-divider v-if="index === current_selected_index" :thickness="5" style="margin-top: 14px;"></v-divider>
                <div v-if="index === current_selected_index" class="introduction_content_container">
                    <div class="toReadBtn font-weight-light" style="font-size: 24px;">阅读</div>
                    <div style="height: 180px; width: 250px;">
                        <v-img
                        height="180"
                        cover
                        src="https://picsum.photos/350/165?random"
                        ></v-img>
                    </div>
                    <p style="padding-left:20px; width: 450px; line-height: 32px; font-size: 14px; color: #BBBBBB;">
                        {{introduction_text}}
                    </p>
                </div>             
            </div>
        </div>
    </div>
</template>
<script lang="ts" setup>
    const current_selected_index = ref(0)
    const blog_list = [
        'Studiopepe&意大利先锋设计',
        'Louisa grey&伦敦简单的优雅',
        '极墅之旅&国内高端民宿设计风向',
        'GoCstudio&西雅图住宅风向',
        'Lotta Agaton&瑞典设计美学风向',
        '极致之墅&Top villas',
        'B.E. Architecture&简单克制澳洲现代建筑',
        '比利时建筑师Nicolas Schuybroek&极简到建筑的本质',
        'Aagnes Studio&墨西哥自然的邀约',
        '极致之墅&中国住宅设计风向'
    ]
    const introduction_text = ' 地球是我们的家园。地球提供真实的材料、温暖的色彩和归属感。地球是我们需要承担责任的地方。室内设计项目引导我们发现我们与地球的联系，唤起我们的和平感。在这个项目中，大自然激发了我们对色彩和材料的选择，并对设计方法进行了仔细和有意识的思考。自然的色调在一个连贯的物质维度中创造出视觉上的连续性。饰面和家具与室内的陶土、沙土和粘土色调相得益彰。暖色调的灯光、天然和实验性的材料增强了我们与地球的联系感。一个悬浮的大月亮是这个装置的焦点，它重现了置身于宇宙中心的感觉。周围的环境让我们的视觉和触觉都倍感舒适。探索互联智能设备、创新材料及其无限应用的真正感官体验。'
    const changeCurrentIndex = (index)=>{
        console.log('old value:' + current_selected_index.value)
        console.log('new value:' + index)
        current_selected_index.value  = index
    }
</script>
<style lang="scss">
.container{
    box-sizing: border-box;
    height: 150%;
    width: 100%;
    padding: 50px;
    display: flex;
    flex-direction: column;
    .navigation_container{
        height: 100px;
    }
    .catalogue_container{
        .introduction_content_container{
            position: relative;
            display: flex;
            margin-top: 20px;
            margin-bottom: 50px;
            height: 20px;
            width: 100%;
            .toReadBtn{
                flex: 1;
                line-height: 1em;
            }
            p{
                letter-spacing: 0.2em;
            }
        }
    }
}
</style>