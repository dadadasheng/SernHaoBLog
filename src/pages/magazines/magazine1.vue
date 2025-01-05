
<template>
    <div class="magazine">
        <div class="cover">
            <div class="navigation">
                <span @click="router.replace('/')">SernHao.Blog</span> | 
                <span @click="router.replace('/architecture')">建筑</span>
            </div>
            <div>
                <h4>
                    比利时建筑师
                </h4>
                <div class="image_2">
                    <v-img
                    width="300"
                    height="200"
                    src="../../images/magazine_1/person_2.png"
                    ></v-img>
                </div>
                <div class="image_3">
                    <v-img
                    width="300"
                    height="400"
                    src="../../images/magazine_1/person_3.png"
                    ></v-img>
                </div>
                <div class="image_1">
                    <v-img
                    width="500"
                    height="400"
                    src="../../images/magazine_1/person_1.png"
                    ></v-img>
                </div>
                <h1>
                    NicolasSchuybroek
                </h1>
                <h2>
                    极简到建筑的本质
                </h2>
                <p>
                    {{Artical.introduction}}
                </p>
            </div>
        </div>
        <article class="article_1">
            <header>
                <span>
                    {{Artical.body[0].title}}
                </span>
            </header>
            <div class="article_image_1">
                    <v-img
                    width="600"
                    height="400"
                    src="../../images/magazine_1/article_1.png"
                    ></v-img>
            </div>
            <main>
                <p>
                    {{Artical.body[0].paragraph}}
                </p>
            </main>
        </article >
        <article class="article_2">
            <div class="article_2_image_1">
                    <v-img
                    width="500"
                    height="1200"
                    src="../../images/magazine_1/article_2.png"
                    ></v-img>
            </div>
            <header>
                <span>
                    {{Artical.body[1].title}}
                </span>
            </header>
            <main>
                <p>
                    {{Artical.body[1].paragraph}}
                </p>
                <div class="image_container">
                    
                </div>
            </main>
        </article>
        <article class="article_3">
            <header>
                <span>
                    {{Artical.body[2].title}}
                </span>
            </header>
            <main>
                <p>
                    {{Artical.body[2].paragraph}}
                </p>
            </main>
        </article>
            <article class="article_4">
            <header>
                <span>
                    {{Artical.body[3].title}}
                </span>
                
            </header>
            <main>
                <p>{{Artical.body[3].paragraph}}</p>
                
            </main>
        </article>
        <article class="article_5">
            <header>
                <span>
                    {{Artical.body[4].title}}
                </span>
                
            </header>
            <main>
                <p>
                    {{Artical.body[4].paragraph}}
                </p>
                
            </main>
        </article>
        <article class="article_6">
            <header>
                <span>
                    {{Artical.body[5].title}}
                </span>
            </header>
            <main>
                <p>
                    {{Artical.body[5].paragraph}}
                </p>
                
            </main>
        </article>
    </div>
</template>
<script setup lang="ts">
import { useTheme } from 'vuetify';
import router from '@/router';
const theme = useTheme()
theme.global.name.value = 'light'
const Artical = 
    {
        head: "极简到建筑的本质",
        introduction: ` Nicolas Schuybroek出生于1981年，在布鲁塞尔长大。受过英语，法语和荷兰语学校的教育，熟练这三国语言，习惯于用这三种语言工作。他的多元文化背景和广泛的旅行以广泛和国际视野滋养他的工作。
                        2011年8月，Nicolas Schuybroek在比利时布鲁塞尔开展自己的设计公司，具有明确的目标：创造和生产以尖锐的细节，工艺和直觉为特征的建筑，内饰和产品，同时保持温暖的感觉。
                        追求永恒的极简主义和明显的简约是他作品的核心，以及对朴素、触觉和原材料的热爱。他的作品毫不费力——只是一种恬静的优雅。
                        Nicolas Schuybroek设计的本质是设想宁静纯净，但又非常温暖和真实的空间。虽然他的建筑经常被描述为修道士和简约主义，但令人惊奇的是，它总是有灵魂。他的作品探索了空间和材料的尖锐视野。大多数人通过严格和背景的方式认识尼古拉斯的手：拥抱建筑形式的精华，从最粗糙的建筑到最小的室内细节。`,
        body:[
            {
                title:'JVC House',
                paragraph:`对于Nicolas Schuybroek来说，设计的挑战是最大限度地扩大房子的面积，为业主的母亲和他们的孩子提供一个多代家庭度假屋。

                        当涉及到城市主义和新建筑项目的形状、材料和体量时，Knokke地区以其保守主义而闻名。该地区的规则使得项目要在建筑中实现当代风格的话比较困难。

                        设计团队找到了一个灵感来自于超大茅草屋顶的解决方案，这可以在90世纪的比利时可以体验到，这种屋顶今天仍然在斯堪的纳维亚和北欧使用。房子是一种当代的诠释，它是一个抽象的家庭度假小屋。

                        Nicolas Schuybroek设计团队试图增强屋子的立体感，在提供隐私感的同时使房子与周围的景观融为一体，塑造一种微妙的扭曲。

                        他们设计了一座需要看起来像一个整体的房子，但它也可以有可以与其他房间翻倍并分开运作的房间，以满足使用房子的三个不同世代的需求，同时赋予房子一种与众不同的风格。`,
            },
            {
                title:'DD House',
                paragraph:`
                    这栋单层房屋是为一个有三个孩子的年轻家庭建造的，Nicolas Schuybroek将其融入土地的缓坡中，营造出更加谨慎的外观，增强了地块的自然美感。

                    一条长长的连续走廊形成了房子的中央流线，连接卧室和起居空间，营造出类似于OV房子的团结感。虽然建筑语言极简且比例协调，但外部材料参考了更本地化的方面：石灰水洗砖和实木块窗框。该项目融入社区，同时为这个年轻家庭的成长保留了非常鲜明的当代特色。

                    Nicolas Schuybroek喜欢在他的项目中使用农场桌子，并通过引入标志性的椅子和周围的物品来赋予它们生命。这所房子让他有机会在大片华丽的土地上应用现代建筑语言，灵感来自废弃的农舍。

                    农舍通常伴随着筒仓和棚屋，所以这些房子里的生活涉及到多个体量的循环，这是设计师在这个和其他项目中应用的一种在生活空间中循环的方式。在该地区丘陵、自然、保存完好的环境中，现有的老农舍几乎与道路相接。

                    当工作室将项目分成两个不同的部分时，他们设法获得了许可：主屋和附属建筑。虽然两者不是同一体量的一部分，但一堵长长的花园墙在物理上和概念上将它们连接起来。

                    他们在两者之间的空间中整合了一个游泳池，创造了一个与西南方向吹来的强风隔绝的僻静绿洲。

                    房子看起来完全不同，这取决于从哪里看它，增强了他们喜欢在项目中巧妙地实现的惊喜和意想不到的感觉。
                `,
            },
            {
                title:'NWJ House',
                paragraph:`该别墅建于1870年代，位于安特卫普，新古典主义的建筑样式给了Nicolas Schuybroek更多的设计可能和发挥空间，在城市街区，借助美丽的后花园，打造一处温暖且拥有乡村生活般的安宁。

                            室内展示了业主收藏的三幅Guy Vandenbranden的画作，除了对艺术的爱好，这所住宅，也是业主对于艺术热爱的明证。

                            从一开始，客户就告诉Nicolas Schuybroek他正在寻找一所完整的房子，从室内设计到家具和艺术品，从最细微的细节开始。

                            这正是设计师喜欢进行的那种项目。于是他们紧密合作，从一开始就做出了正确的选择。从项目开始到结束，他们之间的默契度非常高，这让设计师受到启发，将最大的精力投入到项目中以使其发挥作用，并在保持他们标志性风格的同时突破创造力极限。`,
            },
            {
                title:'The Bath Salon',
                paragraph:`AD Intérieurs 是十年前由 Architectural Digest France 发起的，该平台将十位不同的建筑师和设计师聚集在巴黎，并为他们每个人提供一个房间和“全权”来展示他们的风格和工艺。这让人想起20世纪20年代巴黎的沙龙，允许经常为私人客户工作的艺术家在公共空间展示作品。

                        Nicolas Schuybroek很荣幸能受到邀请，并利用这个机会展示了一个浴室。在某些方面，这是一个不寻常的选择，因为这是一个如此私人的空间，但浴室是人们在房子中投资最多的空间之一，而浴室是一个最有助于营造舒适感的空间。

                        更重要的是，这对设计师来说是一个完美的挑战：如何做一个纯粹的室内项目，同时给它一个强大的建筑维度。对工作室来说，这也是一个机会，让所有杰出的工匠和工匠，如Obumex、Eggermont、Odilon或mform，过去多年来一直和他们在合作，并公开庆祝他们的才华。

                        这个浴室项目没有任何背景，一个“盒子里的世界”。这也是一个没有任何借口的项目，因为没有客户，没有真正的限制。这些通常是非常重要的考虑因素，尤其是在室内设计需要的细节水平。

                        这是一个自由设计的空间项目，以及这种自由带来的能量和动力。这里的板条石让Nicolas Schuybroek想起他一直着迷的装饰艺术细节。

                        设计团队能够创造一个感觉像寺庙的浴室，捕捉在双年展Interieur项目中唤起James Turrell和Constantin Brâncuși的感觉。`,
            },
            {
                title:'Hullebusch',
                paragraph:`设计布景与建造房子、办公室或酒店，甚至设计一个“永远”存在的物体是完全不同的。Nicolas Schuybroek的工作是实现永恒，展览的本质是有时间限制的，但从临时空间建立持久记忆的挑战令他兴奋。受Hullebusch(比利时及海外著名的天然石材品牌)的邀请来设计他们在2018年Interieur双年展上的展览是一个惊喜，因为他们不是主要供应商或通常的供应商。Nicolas Schuybroek想要创造一个隐蔽的、沉思的建筑，与展览厅的其他部分隔开，让人们直接与石头接触。于是设计师想出了一个想法，创建一个矩形的盒子，有一个小开口，可以充满光线。一进入这个空间，人们就会进入一种完全不同的精神状态，在这种状态下，他们会失去所有的时间感。圆形空间的地板上使用了砾石，以减缓步伐，并营造出一种环境，让人们不得不坐下来享受安静，这是从外面嘈杂的展厅中获得的喘息之机。工作室创造了一个圆形的僻静空间，以向对他们的实践产生深远影响的两位艺术家致敬：James Turrell和Constantin Brâncuși 。`,
            },
                {
                title:'JR Apartement',
                paragraph:`Nicolas Schuybroek为他们的布鲁塞尔的客户设计他们位于巴黎的公寓。工作室第一次遇到这个项目是作为一个在四十年不变的重量下起伏的公寓：它非常黑，剩下的紫色油漆被漏水弄脏了，而且非常凌乱。然而，它也散发出令人兴奋的潜力——尤其是考虑到它位于蒙帕纳斯附近第六区雷恩街的高处。工作室表示他们必须彻底改造公寓，开发一个新的方案，创建一个新的循环，引入尽可能多的自然光，并利用高天花板。重建空间的建筑工作相当紧张。现有的布局被彻底改造，将厨房和浴室的位置交换，从之前的三个小房间创造了一个大的生活空间。在这个项目中，材料被严格控制在最低限度。进入公寓，一个完全覆盖着橡木单板的小走廊，让人从巴黎的兴奋中平静下来，并进入室内的其余部分。一盏华丽的1960年Gino Sarfatti灯似乎漂浮在入口走廊迎接游客。当灯开着的时候，这种形式有一些神奇的东西，因为看不到光源，柔软的纹理与该地区木材的原始和公寓的高度相辅相成。厨房位于空间的中心，包裹在同样的拉丝橡木镶板中，中间有一个雕塑般的Carrara大理石柜台。厨房的地板也是大理石的，与相邻客厅的木地板铺设相同的人字形图案，与公寓的其他部分形成了一种节奏感。最后的装饰是复古的法国家具和经典的斯堪的纳维亚灯具。餐厅和客厅中简单而优雅的嵌入式架也为客户提供了展示的机会，分享他们最珍贵的物品，这为空间增添了进一步的温暖。`,
            },

        ]
    }
console.log(router)
console.log(Artical)
</script>
<style scoped lang="scss">
    @font-face {
        font-family: 'LOGO';
        src: url('../../../public/ZhanKuXiaoLOGOTi-2.otf');
    }
    .magazine{
        height: fit-content;
        padding: 50px;
        .cover{
            position: relative;
            height: 900px;
            .navigation{
            margin-bottom: 10px;
            span:hover{
                cursor: pointer;
                }
            }
            h1{
                font-family: 'LOGO';
                color: #5D55E8;
                position: relative;
                font-size: 128px;
                background-color: transparent;
                z-index: 0;
                text-shadow: 1px 1px 2px rgb(255, 255, 255);
            }
            h2{
                position: relative;
                font-size: 64px;
                background-color: transparent;
                z-index: 0;
                margin-bottom: 40px;
            }
            h4{
                color: #5D55E8;
                font-weight: lighter;
            }
            p{
                position: absolute;
                font-size: 14px;
                width: 60%;
                letter-spacing: 2px;
                line-height: 28px;
                background-color: transparent;
            }
            .image_1{
                position: absolute;
                top: 50px;
                right: 100px;
                z-index: 0;
            }
            .image_2{
                position: absolute;
                top: 100px;
                right: 600px;
                z-index: 0;
            }
            .image_3{
                position: absolute;
                top: 300px;
                right: 0px;
                z-index: 0;
            }
        }
        .article_1{
            position: relative;
            header{
                position: relative;
                margin-bottom: 40px;
                span{
                    font-size: 36px;
                }
                
            }
            main{
                position: relative;
                p{
                    width: 50%;
                    font-size: 14px;
                    letter-spacing: 2px;
                    line-height: 28px;
                    background-color: transparent;
                }
            }
            .article_image_1{
                position: absolute;
                top: -220px;
                right: 50px;
            }
        }
        .article_2{
            position: relative;
            z-index: 1;
            padding: 50px 0;
            transform: translateX(-50px);
            header{
                width: 65%;
                background-color: rgba(128, 128, 128, 0.329);
                padding:40px 50px;
                span{
                    font-size: 36px;
                }
            }
            main{
                p{
                    padding: 20px 50px;
                    width: 65%;
                    font-size: 14px;
                    letter-spacing: 2px;
                    line-height: 28px;
                    background-color: rgba(128, 128, 128, 0.329);
                }
            }
            .article_2_image_1{
                position: absolute;
                top: 10px;
                right: -100px;
                z-index: -1;
            }
        }
        .article_3{
            header{
                margin-bottom: 40px;
                span{
                    font-size: 36px;
                }
            }
            main{
                p{
                    width: 50%;
                    font-size: 14px;
                    letter-spacing: 2px;
                    line-height: 28px;
                    background-color: transparent;
                }
            }
        }
        .article_4{
            header{
                margin-bottom: 40px;
                span{
                    font-size: 36px;
                }
            }
            main{
                p{
                    width: 50%;
                    font-size: 14px;
                    letter-spacing: 2px;
                    line-height: 28px;
                    background-color: transparent;
                }
            }
        }
        .article_5{
            header{
                margin-bottom: 40px;
                span{
                    font-size: 36px;
                }
            }
            main{
                p{
                    width: 50%;
                    font-size: 14px;
                    letter-spacing: 2px;
                    line-height: 28px;
                    background-color: transparent;
                }
            }
        }        
        .article_6{
            header{
                margin-bottom: 40px;
                span{
                    font-size: 36px;
                }
            }
            main{
                p{
                    width: 50%;
                    font-size: 14px;
                    letter-spacing: 2px;
                    line-height: 28px;
                    background-color: transparent;
                }
            }
        }
    }
</style>