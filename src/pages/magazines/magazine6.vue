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
        head: "B.E. Architecture&简单克制澳洲现代建筑",
        introduction: `B.E. Architecture的项目深入了解情景和建筑物的用户体验，使其具有意义，并且随着时间的推移将继续保持相关性。他们的作品已经获得众多奖项的认可，并在澳大利亚和海外广泛出版。

                        公司在创造精密，永恒的建筑方面的经验使他们赢得了同行的尊重，更重要的是赢得了客户的尊重。B.E. Architecture.建筑在住宅和商业空间建筑方面有着悠久的历史。 `,
        body:[
            {
                title:'Erskine Street Residence',
                paragraph:`位于南墨尔本的Erskine Street Residence由B.E Architecture的Andrew Piva和Duncan McLeary设计，是一个平衡几何造型和柔和材质的静谧空间。

                住宅坐落在Middle Park一排维多利亚风格工人小屋的尽头，白色现浇混凝土和石灰石外观呈现出大胆的几乎没有窗户的设计，与街景形成鲜明对比。住宅包括一个主卧、独立客房、健康空间和一个宽敞的酒窖，整体风格融合了日本和19世纪巴黎建筑的独特元素。

                室内设计延续了外部材质的柔和感，白色混凝土与浅灰色Bolzano石灰石相结合，从地板到天花板形成了统一的装饰，烘托出业主的艺术藏品。

                橡木的木工设计和滑动屏风为极简空间增添了温暖，铸铁散热器和带有链条火幕的混凝土壁炉等细节则致敬了早期现代主义建筑，赋予了空间一种神圣的宁静氛围。天窗带来充足的自然光，照亮了一系列围墙花园，园中栽种了黑松、枫树和盆栽的榉树，让空气感与建筑的坚固外壳形成对比。

                Erskine Street Residence融合了永恒设计和感官空间，营造出一处静谧的避风港。由B.E Architecture负责建筑、室内设计和风格塑造，Dome Builders负责施工，这所住宅展现了坚固与安宁的巧妙平衡，成为都市生活中的理想栖息之所。`,
            },
            {
                title:'Shakespeare Grove House',
                paragraph:`Shakespeare Grove 住宅坐落在墨尔本最重要的遗产住宅区之一。设计强调手工艺和定制细节，融合了现代和古老的材料。

                项目成功的一个关键因素是在同一栋建筑中创造出两个截然不同的部分。如果将它们放在一起体验，就会让人联想到一个时代住宅的扩建部分。

                前部设有主卧室套房、书房和正式客厅，设有毡衬墙壁和图案木天花板。相比之下，后部包含主要的起居空间和额外的卧室，墙面采用渲染混凝土，并配有全铜厨房。在整个项目中，工匠之手显而易见。经过精心考虑的细节在房屋的不同区域之间营造出一种凝聚力和平衡感。 

                客户的主要关注点是建造一栋随着家庭成长而与他们的生活息息相关的房子。客户认为，建筑应该提升人们的生活品质，因此在空间和风格上都应该是永恒的。

                澳大利亚的住宅建筑大多采用大面积玻璃窗并注重景观，而这些客户则希望住宅朝内，窗户较小，并有足够的墙面空间摆放艺术品。`,
            },
            {
                title:'About B.E. Architecture',
                paragraph:`由Broderick Ely, Jonathon Boucher And Andrew Piva领导的B.E.建筑团队年轻，充满活力，该公司以其精密的住宅和商业项目而闻名，拥有一支从事建筑，景观，室内装饰，家具，照明和物体设计的多学科团。

                Broderick Ely（中）作为B.E. Architecture的设计总监，将创意设计理念与高度亲身实践的方法相结合，创造出具有个性的建筑。他不断研究和开发新的概念，通过整合创新技术和历史悠久的建筑技术，寻找合适的设计解决方案来表达客户的兴趣。他活跃在澳大利亚和海外的美术界，经常策划和委托重要的艺术作品进入B.E的项目。

                Jonathon Boucher作为B.E. Architecture的联合创始人兼总监，Jonathon是一位架构师，他既了解设计过程，又了解与主要利益相关方和委员会合作的大局，帮助客户实现其目标，即使在严格的限制下也能实现富有远见的项目。`,
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