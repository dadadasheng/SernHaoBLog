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
        head: "Studiopepe 意大利先锋设计",
        introduction: ` `,
        body:[
            {
                title:'Terra 展厅',
                paragraph:`自然的色调在一个连贯的物质维度中创造出视觉上的连续性。饰面和家具与室内的陶土、沙土和粘土色调相得益彰。暖色调的灯光、天然和实验性的材料增强了我们与地球的联系感。

                一个悬浮的大月亮是这个装置的焦点，它重现了置身于宇宙中心的感觉。周围的环境让我们的视觉和触觉都倍感舒适。探索互联智能设备、创新材料及其无限应用的真正感官体验。地球是我们的家园。地球提供真实的材料、温暖的色彩和归属感。地球是我们需要承担责任的地方。

                室内设计项目引导我们发现我们与地球的联系，唤起我们的和平感。在这个项目中，大自然激发了我们对色彩和材料的选择，并对设计方法进行了仔细和有意识的思考。`,
            },
            {
                title:`Avart
                    Boutique
                    In
                    Lugano`,
                paragraph:`这是一家位于瑞士卢加诺市中心的一家时尚精品店，室内以自然的色调、柔软的几何形状、戏剧性的材料对比和丰富的纹理为主要特征，以此传递一种迎接顾客到访的氛围，体现出精致的、具有当代女性属性的气质。

                墙壁和地面被裸色的微沙肌理所装饰，创造出一个中性与感性的表皮，丰富了内部空间的形体表现。石膏的粗大圆柱和螺旋楼梯，像一条连续的缎带，连接着上下两层的精品店，并成为了室内关键性的雕塑元素。

                室内用纯大理石来加强了它的纹理和强烈的色彩，以此来点缀其中性的色调，带出他们的各种深浅和色彩。Travertino Silver覆盖了入口立面和室内陈设，而粗糙和不规则的Smeraldo Onyx和Fusion Pink大理石面板被改造成展示桌，它们未完成的形式为室内增加了复杂性和质量。

                灰色熔凝玻璃幕墙将空间划分为不同的功能区。玻璃也被用作为装饰元素，如Barovier & Toso的大型枝形吊灯，Venini贴花点缀了装修区域。

                Adrianna和Chiara与当地的Bedano工匠、Veragouth和Xilema细木工合作，实现了关键的空间元素。天然黄铜的衣架悬挂在墙壁上，在中性背景下形成图形的形状。珍贵的粉红色镜子覆层与缎面黄铜型材和石灰石把手打开，揭示了一个粉红色皮革和地毯的整个室内装潢。`,
            },
            {
                title:'About Studiopepe',
                paragraph:`Studiopepe是一家位于米兰的设计公司，由Arianna Lelli Mami和Chiara Di Pinto于2006年创立。这两位出色的设计师凭借其多元化和多层次的设计美学，以及富于远见的多学科设计方式，开创出独特的设计理念。

                Studiopepe是一个以折衷主义和多层视角著称的设计工作。基于实验，引用不寻常的元素，寻求独特性和尊重客户的个性。她们的复古风格的外观以现代风格重新诠释了经典。使用柔和的色调和柔和的色彩，美丽而豪华的材料和永恒的设计作品，实现了非常复杂和温暖的氛围。

                Studiopepe的项目的特点是他们的情感和审美影响，融合了视觉的严谨性，以及不断寻找当代元素和语言的感染力。灵感均来自坚实的设计经验，一起实现了具有强烈情感价值的概念和项目。`,
            },
        ]
    }
</script>
<style lang="scss">
    
</style>