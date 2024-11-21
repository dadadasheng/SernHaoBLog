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
        head: "GoCstudio西雅图住宅风向",
        introduction: ` `,
        body:[
            {
                title:'西雅图Sound House',
                paragraph:`Sound住宅位于西雅图的木兰社区，在市中心西北部的高架半岛上，普吉特海湾和西雅图市中心的美景尽收眼底。该项目是一座占地5500平方英尺的独户住宅，将取代建于20世纪20年代的现有房屋。新建筑所在的地块顶部原有一块高地。 事务所设计了一系列阶梯花园和小径，在斜坡上形成一个用餐和泳池露台。场地的驱动因素之一是几乎 360 度的景观，设计使每一层的景观都能得到最大程度的利用。该住宅的设计方案非常独特，因为它需要容纳一个由两个成年人和六个孩子组成的大家庭。该住宅的设计目的是让所有家庭成员都能享受到充足的生活空间，并能通往许多室外露台和屋顶平台--打造一个适合聚会的住宅至关重要。 从普吉特海湾的广阔景色、播放的音乐以及居住在这所房子里的六个孩子来看，"Sound House "这个名字再合适不过了。`,
            },
            {
                title:'Western Studio',
                paragraph:`位于美国西雅图一个摄影工作室Western Studio，由当地的室内设计工作室GoCstudio设计。Western Studio是为喜欢摄影和招待客人的客户而设计的家和工作室。这个92.9平方米的开放式单元位于西雅图贝尔镇附近的一座商业建筑内。该项目的目标是将厨房、浴室和睡眠区重新设计为一个紧凑的多功能盒子，使其余空间成为开放的平面和适应性。一排橱柜、灰色的厨房电器和一扇滑动木门正对着用染色胶合板包裹的整体盒子。建筑面向开放式的生活区，在改造过程中，生活区被部分改造为摄影工作室。为了将空间改造成工作室，客户建议建造一个可调节的系统，以容纳锁子甲幕布，在拍摄期间可以很容易地替换为摄影背景。垂直的金属板连接在天花板上的轨道上，也以暴露的管道为特色，呼应公寓楼的工业历史。盒子的一角是一间紧凑的卧室，墙壁上覆盖着毛毡。在单元内部，床堆叠在木质储物柜的顶部，上方设有天窗，为狭窄的空间提供光线和通风。浴室里的深色威尼斯抹灰与盒子外部使用的染色胶合板的色调相匹配。这间密闭房间里的设备包括一个定制雕刻的Jatoba水槽和梳妆台，以及一个配备变色灯的雨淋头。为了增加存储和实用空间，工作室在盒子结构上方设计了一个“阁楼”层，可以从侧门或厨房顶部的一排橱柜进入。`,
            },

        ]
    }
console.log(router)
console.log(Artical)
</script>
<style lang="scss">
    
</style>