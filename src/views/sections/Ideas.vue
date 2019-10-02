<template>
    
    <div id="section-ideas" class="section">
        <div class="container">
            <div class="md-layout">
                <div class="md-layout-item md-size-80 md-xsmall-size-100 mx-auto">
                    <h2 class="text-center title">主題發想</h2>
                    <p class="description">
                        對「匱乏」產生意識，是人們合作的契機；在合作中，人們得以一同探索共好生活的想像。
                    </p>
                    <p class="description">
                        我們邀請各位一同針對食農相關議題，提出具有合作精神的問題解決方案，
                        您可以在這裡尋找靈感、找志同道合的夥伴組隊參與或者針對特定食農問題提出你的看法（挖坑）、吸引有興趣的人加入（填坑）!
                    </p>
                    
                </div>
            </div>

            <div class="md-layout">
                <div class="md-layout-item md-size-80 md-xsmall-size-100 mx-auto">

                    <!-- <div> -->
                        <b-card-group columns>
                            <b-card title="農業生產" :img-src="getImgURL('img/topic1_coa.jpg')" img-alt="Image" img-top >
                                <b-card-text>
                                    在氣候變遷、能源依賴、人口增長、通路規格化等挑戰下，現代農民如何利用資訊技術，幫助農民以友善環境的方式穩定生產出質量兼具的食物來餵飽全世界？
                                </b-card-text>
                                <p class="text-center">
                                    <b-button variant="success" @click="goToPage('topic')">更多討論</b-button>
                                </p>
                            </b-card>

                            <b-card title="在地生活" :img-src="getImgURL('img/topic3_coa.jpg')" img-alt="Image" img-top >
                                <b-card-text>
                                    人們在鄉村、在都市，用各自的方法與土地一起生活。無論都市或鄉村，有農業的地方即能創造在地生活。在創造理想的在地生活的過程中，人們會遭遇哪些困難？需要哪些協助？
                                </b-card-text>
                                <p class="text-center">
                                    <b-button variant="success" @click="goToPage('topic')">更多討論</b-button>
                                </p>
                            </b-card>

                            <b-card title="食農教育" :img-src="getImgURL('img/topic5_coa.jpg')" img-alt="Image" img-top >
                                <b-card-text>
                                    農業未來掌握在下一代，而教育，則是世代溝通的重要管道。農耕者如何與消費者溝通？我們又如何與孩子對話？我們需要新的媒介、新的方法、新的工具。
                                </b-card-text>
                                <p class="text-center">
                                    <b-button variant="success" @click="goToPage('topic')">更多討論</b-button>
                                </p>
                            </b-card>

                            <b-card title="農產運銷" :img-src="getImgURL('img/topic2_coa.jpg')" img-alt="Image" img-top >
                                <b-card-text>
                                    除了生產外，農產品收穫後清洗、處理、加工、集貨、包裝、物流、大盤商、中盤商、最後才經由通路商進到消費者的生活之中，整個產業鏈正在悄悄轉變。產業的未來，由你來打造。
                                </b-card-text>
                                <p class="text-center">
                                    <b-button variant="success" @click="goToPage('topic')">更多討論</b-button>
                                </p>
                            </b-card>

                            <b-card title="生態永續" :img-src="getImgURL('img/topic4_coa.jpg')" img-alt="Image" img-top >
                                <b-card-text>
                                    要增加農業永續性並不需要完全捨棄現有的慣行農業機制，只要能夠一點一點改善，就能慢慢使農業往永續發展的目標前進。讓我們用新的工具幫助人們上手，推動改變。
                                </b-card-text>
                                <p class="text-center">
                                    <b-button variant="success" @click="goToPage('topic')">更多討論</b-button>
                                </p>
                            </b-card>

                            <b-card title="標章溯源" :img-src="getImgURL('img/topic6_coa.jpg')" img-alt="Image" img-top >
                                <b-card-text>
                                    處於資訊「透明」的時代，人們應該如何理解巨量資訊？產銷間的資訊與知識落差如何弭平？市面上各種標章認證機制又該如何讓消費者認識，並進而取得信賴？或者，我們需要何種全新的溯源方式？
                                </b-card-text>
                                <p class="text-center">
                                    <b-button variant="success" @click="goToPage('topic')">更多討論</b-button>
                                </p>
                            </b-card>

                            <b-card title="無法歸類的各種農業坑" :img-src="getImgURL('img/topic7_coa.jpg')" img-alt="Image" img-top>
                                <b-card-text>
                                    
                                </b-card-text>
                                <p class="text-center">
                                    <b-button variant="success" @click="goToPage('topic')">更多討論</b-button>
                                </p>
                            </b-card>
                        </b-card-group>
                    <!-- </div> -->

                </div>
            </div>


        </div>
    </div>

</template>

<script>
export default {

    methods: {

        getImgURL (img)
        {
            return process.env.BASE_URL + img
        },

        goToPage ( topic )
        {
            if (topic)
            {
                window.open('https://www.facebook.com/groups/412776526095442/?epa=SEARCH_BOX', '_blank');
            }
        },
    }
}
</script>

<style lang="scss" scoped>

</style>