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
        head: "Aagnes Studio&墨西哥自然的邀约",
        introduction: ` Aagnes Studio的作品常常围绕着事物对立面之间的相互作用而进行，如传统和现代，无论本地化或是全球性，所有的一切都有着强烈的地方意识。这种精神使建筑与场地得以充分接触并对产生一种尊重，最终构建出满足于人们日常生活、思考和休息的场所。
            另一方面，Aagnes Studio工作室在每个项目中使用不同的或特殊的元素必然能够产生迥异的表达语境：随着光线的变化，建筑的色调、肌理、表皮、感知也会随之发生改变，光被作为一种独特的自然形式存在，而植物色调的使用则完美地诠释了“自然之色”的核心要义。`,
        body:[
            {
                title:'Casa Cedros House',
                paragraph:`该项目坐落于墨西哥，由Aagnes室内设计工作室完成。他们的作品常常围绕着事物对立面之间的相互作用而进行，如传统和现代，无论本地化或是全球性，所有的一切都有着强烈的地方意识。

                这种精神使建筑与场地得以充分接触并对产生一种尊重，最终构建出满足于人们日常生活、思考和休息的场所。

                Aagnes的设计使命是一次对当代美学的“邀请”；是一种内省的乐趣，能够让人停下来思考。带着“反思”的认知来审视工作室的作品是必要的，他们的风格可以被作为是一种持续性的对话：在传统与现代、当地与全球趋势、历史与永恒之间展开。

                Aagnes将天然材料和自然色调作为项目的主要元素进行运用，空间中所见的每一件单品、每一种材料都是对周围社区的传统文化表示致敬，也正因为他们对于当地手工艺的尊重，才使这些传统得以延续。

                对于工作室而言，在每个项目中使用不同的或特殊的元素必然能够产生迥异的表达语境：随着光线的变化，建筑的色调、肌理、表皮、感知也会随之发生改变，光被作为一种独特的自然形式存在，而植物色调的使用则完美地诠释了“自然之色”的核心要义。`,
            },
            {
                title:'Viatura Omun Hotel',
                paragraph:`Casa Los Tigres，这是一座海边的房子，体现了墨西哥独特的亲生物设计语言，是César Béjar Studio与建筑师Fernando Sánchez合作设计的。

                Casa Los Tigres位于墨西哥西海岸的海滨小镇新巴亚尔塔。一年中有一半的时间，这里的气候宜人温暖，不使用空调，允许建筑物向室外开放。在一年中的另一半，当温度更高，湿度也更高时，随着植被的蓬勃发展，景观也发生了变化。

                这种气候让csamar和Fernando决定将室内和室外空间的比例均匀化，并在两个领域之间进行一些优雅的过渡。整个花园都充满了雨季的气息。

                除了对气候做出反应，César Béjar和Fernando还整合了该地区的典型建筑特征，其中之一是烧制粘土的屋顶和地板。这种自然纹理的材料与其他相同性质的材料结合在一起，包括手工制作的砖块和瓷砖，以及染色的热带木材，所有这些都来自当地。

                “我们不追求闪亮的饰面——相反，我们对使用当地的有机材料很感兴趣，”César Béjar说。`,
            },
            {
                title:'关于设计 About Aagnes Studio',
                paragraph:`具备极高职业敏感度的Aagnes Studio是一家位于墨西哥瓜达拉哈拉的家具和建筑设计工作室，他们对作品中所呈现的工艺和细节有着极致的追求，包括肌理、光感、使用的材料属性、寂静的氛围和未来居住的空间情境。

                Aagnes Studio的设计使命是一次对当代美学的“邀请”；是一种内省的乐趣，能够让人停下来思考。带着“反思”的认知来审视工作室的作品是必要的，他们的风格可以被作为是一种持续性的对话：在传统与现代、当地与全球趋势、历史与永恒之间展开。

                为了展现其美学，Aagnes Studio 充分利用了形状和空间两大支柱。用于项目的物体、道具和部件源自其自己的想象力，使之与其空间的环境相互呼应。`,
            },
            {
                title:'',
                paragraph:``,
            },
        ]
    }
</script>
<style lang="scss">
    
</style>