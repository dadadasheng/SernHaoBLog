<template lang="">
    <div>
        <span @click="router.replace('/')">SernHao.Blog</span> | 
        <span @click="router.replace('/architecture')">建筑</span>
    </div>
    <div>
        <h1>
            {{Artical.head}}
        </h1>
        <p>
            {{Artical.introduction}}
        </p>
    </div>
    <div>
        <article>
            <header>
                {{Artical.body[0].title}}
            </header>
            <main>
                {{Artical.body[0].paragraph}}
            </main>
        </article>
        <article>
            <header>
                {{Artical.body[1].title}}
            </header>
            <main>
                {{Artical.body[1].paragraph}}
            </main>
        </article>
        <article>
            <header>
                {{Artical.body[2].title}}
            </header>
            <main>
                {{Artical.body[2].paragraph}}
            </main>
        </article>
    </div>
</template>
<script setup lang="ts">
import router from '@/router';
const Artical = 
    {
        head: `Lotta Agaton 瑞典设计美学风向`,
        introduction: ` `,
        body:[
            {
                title:`斯德哥尔摩

                        Apartment TS`,
                paragraph:`Oscar地产最新的住宅综合体是位于斯德哥尔摩的令人印象深刻的建筑地标79 & Park，由丹麦建筑师Bjarke Ingels设计，并由Lotta Agaton Interiors进行室内设计，下面是令人惊叹的观景公寓的内部情况。

                这座以纽约为灵感的公寓拥有巨大的落地窗，以及裸露的柱子和横梁。让人联想到苏荷区和布鲁克林区的世纪之交物业的工业粗糙感，用温暖的材料调色板将木质元素和纹理饰面融合在一起，使之变得柔和。观景公寓以标志性的家具和照明设计、雕塑般的陶瓷和引人注目的艺术作品，形成了优美的风格。

                客厅优雅而温馨，摆放着Charlotte Perriand设计的Plana咖啡桌和Living Divani设计的圆形Piero Lissoni扶手椅。Poul Kjærholm设计的精致的PK 24 Chaise休闲椅与Axel Einar Hjorth设计的NK Utö边桌并列。

                许多美丽的陶瓷作品和书籍来自Dusty Deco，这是一家位于斯德哥尔摩的商店，销售来自世界各地的折衷主义珍品。`,
            },
            {
                title:`斯德哥尔摩
                        Apartment TS`,
                paragraph:`这是才华横溢的艺术总监Therese Sennerholt在斯德哥尔摩的房子。Therese Sennerholt和Lotta Agaton一起参与了这个项目。Lotta Agaton帮协助Therese统一了材料和色调的调色板。

                这所房子的一些独特的作品是：由Daniel Östman设计的日间床，来自Santa & Cole的Cesta台灯、PK 24椅子、Superstudio为Zanotta设计的办公桌Quads，这些都是工作室和Therese Sennerholt精心挑选的`,
            },
            {
                title:'About Lotta Agaton Interiors',
                paragraph:`Lotta Agaton Interiors是斯堪的纳维亚地区领先的室内设计工作室之一，由Lotta Agaton创立于2004年，并与多学科团队Lotta Agaton Interiors合作开展商业造型项目，开发内部概念以及房地产开发项目，为私人住宅和商业空间提供室内设计。每个项目都是量身定制的，以满足客户的需求。

                Lotta Agaton拥有超过20年的室内设计经验，包括造型，创意指导和许多国际品牌的咨询。作为Residence杂志的共同创始人，Agaton拥有深厚的编辑合作知识和良好的视觉沟通的影响。

                Lotta Agaton工作室的核心是坚定不移的信念，无论是在家中，商业空间还是图像上，精心策划的空间为人们带来的积极影响。 `,
            },
        ]
    }
console.log(router)
console.log(Artical)
</script>
<style lang="scss">
    
</style>