<template>
    
    <div id="section-result" class="section">
        <div class="container">
            <div class="md-layout">
                <div class="md-layout-item md-size-80 md-xsmall-size-100 mx-auto">
                    <h2 class="text-center title">活動成果</h2>

                    

                    <b-card class="github-card">
                        <h3>2019 食農合作松決選參加作品</h3>
                        <b-card-text>
                            參加團隊的成果皆開源上傳在 Github。
                            <md-button href="https://github.com/Coopathon2019" target="_blank"
                                    class="md-success md-lg block-text" style="float: right;">
                                2019 食農合作松 Github
                            </md-button>
                        </b-card-text>
                    </b-card>

                    <br>
                    <hr>
                    <br>

                    <b-row>

                        <b-col md="6" v-for="(post, idx_p) in results" :key="idx_p">
                            <b-card >
                                <b-card-img top :src="post.pic" :alt="post.alt" @click="goToPage(post.link)" class="clickable"></b-card-img>
                                <b-card-title class="text-center">{{ post.title }}</b-card-title>
                                <b-card-text>
                                    <div v-html="post.content"></div>
                                    <div class="text-center post-button">
                                        <b-button variant="outline-success" @click="goToPage(post.link)">看詳細內容</b-button>
                                    </div>
                                </b-card-text>
                            </b-card>
                        </b-col>

                    </b-row>
                    
                </div>
            </div>

            
            


        </div>
    </div>

</template>

<script>
export default {
    data () {
        return {
            results: [
                {
                    title: '【 2019 食農合作松 - 活動大合照 】',
                    content: `
                        活動落幕，大成功！
                        恭喜獲獎團隊以及感謝各位用心投入參與，期待未來再見！
                    `,
                    pic: './img/pic/75429435_2563541830391375_4675126568039743488_o.jpg',
                    link: 'https://www.facebook.com/agriweather/posts/2563546620390896',
                    alt: '活動大合照',
                },
                {
                    title: '【 評審講評與頒獎 - 直播影片 】',
                    content: `
                        評審講評與頒獎時間！
                    `,
                    pic: './img/pic/頒獎.JPG',
                    link: 'https://www.facebook.com/agriweather/videos/526311624587593/',
                    alt: '評審講評與頒獎',
                },
                {
                    title: '【 黑客松決選 - 直播影片 】',
                    content: `
                        經過24小時的瘋狂黑客松後，現在開始決選囉！
                    `,
                    pic: './img/pic/頒獎.JPG',
                    link: 'https://www.facebook.com/agriweather/videos/3033504316664043/',
                    alt: '黑客松決選',
                },
                {
                    title: '【 開幕論壇 Part 2. - 直播影片 】',
                    content: `
                        講者1：社大全促會秘書長 楊志彬<br>
                        講者2：上下游創辦人 馮小非
                    `,
                    pic: './img/pic/論壇02.JPG',
                    link: 'https://www.facebook.com/agriweather/videos/2784805871575680/',
                    alt: '開幕論壇 Part 2',
                },
                {
                    title: '【 開幕論壇 Part 1. - 直播影片 】',
                    content: `
                        講者：菲律賓 Cropital 創辦人 Ruel Amparo<br>
                        ( 譯者：顏瑜萱 Shirley Yen )
                    `,
                    pic: './img/pic/論壇01.JPG',
                    link: 'https://www.facebook.com/agriweather/videos/2784805871575680/',
                    alt: '開幕論壇 Part 1',
                },
            ]
        }
    },
    methods: {

        goToPage (url)
        {
            window.open( url )
        },

    }
}
</script>

<style lang="scss" scoped>

.github-card
{
    background-color: #cceeee !important;
}

.post-button
{
    margin: 10px;
}

</style>