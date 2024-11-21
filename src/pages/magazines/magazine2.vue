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
        head: "Louisa grey 伦敦简单的优雅",
        introduction: ` Louisa Grey的风格源于她个人想要创造平静、低调的奢华内饰的愿望。因此，她总是试图在设计领域中创造一种“简单的优雅”或者更确切地说是一种自然的、进步的美学。她多年前就开始觉得自己被被更简约的美学所吸引，这种美学能够在物理空间和生活在其中的人们之间创造和谐。`,
        body:[
            {
                title:'葡萄牙 Armadillo&Co Showroom',
                paragraph:`
                            Armadillo&Co Showroom
                            House Of Grey的设计师Louisa Grey与地毯品牌公司Armadillo&Co合作设计了他们位于葡萄牙里斯本的展厅。Armadillo＆Co推出了埃及系列背后的统一理念和安静奢华，并探索安静的环境是如何唤起幸福感的。

                            Louisa Grey认为慢生活的文化将会发生变化，在慢节奏的生活中，人们会考虑自己所买的东西，以及周围的材料对人的影响。Louisa Grey觉得埃及系列带来了舒适感，给人以朴实的感觉，而这正是他在House Of Grey致力于实现的设计原则，这些原则将哲学融合在一起。既要尊重功能又要兼顾美学，以激发家中安静，低调的奢华。

                            Louisa与House of Grey的合作专注于一种优雅的简单感，这能唤起一种平静和幸福的感觉，这又与Armadillo & Co公司及其强烈的道德标准产生了共鸣。

                            Armadillo＆Co推出的地毯不单具有灵魂还有完整性，既尊重当地的文化和建筑历史。从天然的羊毛和黄麻材料的运用，到对当地工匠使用手工制作的认可，正如Louisa所反映的那样，“手工元素构成了产品的支柱”。`,
            },
            {
                title:`Louisa Grey House 伦敦`,
                paragraph:`House of Grey接管了伦敦北部一栋优雅的联排别墅，并用它展示了新兴的本地和国际设计师，艺术家和制作人的作品。他们的作品Louisa Grey House，经过设计师的精心策划，注重手工和天然材料，使结果温暖，优雅且沉稳。这毫无疑问的将是所有人都梦寐以求的理想家园。
                            在她探索所“软斯堪的纳维亚风格”的过程中，她暗示了下一个室内设计大趋势是什么样子。正如她之前所说的，当前对光明和喧嚣模式的关注，仅仅是对不稳定的政治状态的反应。但这一切都会过去的，取而代之的将是一种新的纹理厚重的外观，注重舒适和温暖，回归到更传统的中性色色调，辅以蓝色和各种绿色色调。
                            在Louisa Grey House的设计中，工作室在住宅内就加入了一些令人感到温暖的色调。客厅内设计了大面积的玻璃窗，可以将更多的光引入到室内，盆景的插入让整个空间带有一种回归自然的感觉，提升了氛围感。`,
            },
            {
                title:`About House Of Grey`,
                paragraph:`House Of Grey是一家位于伦敦北部城市的室内设计工作室，专注于舒适住宅和商业项目的室内设计，由创始人Louisa Grey成立于2013年。工作室旨在增进幸福感和美感，尽可能纳入当地来源的高质量，自然和可持续材料，并设计出可以补充人们直观工作和生活方式的空间，并随着人们需求的变化而不断发展。
                Louisa Grey毕业于伦敦切尔西艺术与设计学院并获得学位，至今拥有超过20年的室内设计经验，这些经验造就了她沉着冷静的个人审美。Louisa Grey以其强烈的室内空间布局感而闻名，她开发了一种独特的风格，使她走在人群的前面。`,
            },

        ]
    }
</script>
<style lang="scss">
    
</style>