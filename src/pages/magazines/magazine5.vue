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
    </div>
</template>
<script setup lang="ts">
import router from '@/router';
const Artical = 
    {
        head: "极致之墅&Top villas",
        introduction: ` `,
        body:[
            {
                title:'伦敦The Sessile House',
                paragraph:`Way of Life在伦敦托特纳姆哈利推出其最新住宅项目The Sessile，由前Soho House设计总监Linda Boronkay操刀设计。

                该项目为租户带来奢华设计与酒店式配套设施的结合，营造更高品质的生活方式。住户可享健身房、宁静的瑜伽室、私人用餐区以及屋顶温室等设施，尽览伦敦全景，提供舒适与精品体验的完美融合。

                Linda Boronkay的设计为The Sessile注入独特的优雅与格调，以大理石、柔和木材及精选艺术作品点缀空间。灵活的布局便于多功能使用，大露台和落地窗最大化引入自然光。设计灵感来自后现代及历史艺术形式，空间内融入了图形饰面、定制霓虹艺术品和大胆的色彩，营造出既高雅又温馨的氛围。

                在The Sessile，社区感是核心。通过共用空间和创意活动，住户可以在精心设计的环境中彼此联结。周边的公园与本地商户进一步提升了社区的归属感，使The Sessile成为伦敦高端租赁市场中独具特色的选择。`,
            },
            {
                title:'巴黎Montaigne House',
                paragraph:`这套不拘一格的公寓位位于巴黎时尚地带的中心，由 Hauvette & Madani 公司设计，为一位对艺术充满热情的客户，将历史的华丽与现代的俏皮融合在一起。

                设计通过精心修复的模子和飞檐保留了豪斯曼时期的优雅风格，同时大胆采用了现代美学。其中最引人注目的是充满活力的粉色和绿色厨房，Fornace Brioni 的复古瓷砖衬托着引人注目的绿色 La Cornue 烤箱和粉色橱柜，与公寓的古典特色形成了鲜明的对比。

                这座充满艺术气息的住宅反映了客户的独特风格，为她不断变化的收藏精心设计了平衡空间。

                从弧形入口大厅的门到理查德-佩杜兹（Richard Peduzzi）定制的家具，稻草镶嵌工艺将每个房间连接起来，创造出一种触觉上的整体感。

                在主起居室，复古和现代家具的搭配与 Miriam Cahn 的艺术品相得益彰，而 Erwin Wurm 的天花板雕塑则增添了大胆的变化。让-米歇尔-弗兰克（Jean-Michel Frank）的复古椅子、定制家具和现代艺术品的交相辉映，勾勒出住宅的独特魅力和个性。

                每个房间的纹理、色彩和形式都层次分明。从莎拉-克劳纳（Sarah Crowner）在用餐区设计的图形壁炉到浴室中雕刻的绿色大理石，设计突出了结构和装饰的艺术性。

                Hervé van der Straeten 设计的吧台和餐桌上弧形流畅的线条与整个设计相呼应，在丰富多样的设计中保持了连续性。这间巴黎公寓的色彩和形式都表现得生动活泼，让永恒和非传统和谐统一。`,
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