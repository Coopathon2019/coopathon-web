<template>
    <div id="page-top" class="wrapper">

        <parallax id="section-landing" class="section page-header header-filter" :style="headerStyle">
            <div class="container">
                <div class="md-layout">
                    <div class="md-layout-item md-size-70 md-small-size-90 md-xsmall-size-100">
                        <h1 class="title">
                            2019 食農合作松
                        </h1>
                        <div class="sub-title">
                            在共創中尋找永續
                        </div>
                        <div class="sub-title">
                            Coopathon 2019 : Food in Sustainability
                        </div>
                        <br />
                        <!-- <md-button href="#" class="md-success md-lg block-text" target="_blank">
                            <i class="fas fa-angle-double-right"></i> 報名辦法
                        </md-button> -->
                        <!-- <md-button href="https://coopathon2019.kktix.cc/events/54065dca" target="_blank"
                                   class="md-rose md-lg block-text faa-horizontal animated">
                            馬上報名
                        </md-button> -->
                        <!-- <md-button :href="getImgURL('files/初選入圍名單.jpg')" target="_blank"
                                   class="md-rose md-lg block-text faa-horizontal animated">
                            初選名單
                        </md-button> -->
                        <!-- <md-button href="https://docs.google.com/forms/d/e/1FAIpQLSfnhuQXL9xbFqydo345QlgsE1jJViqRKyuaGN1kAyoz5t9Y2w/viewform" target="_blank"
                                   class="md-rose md-lg block-text faa-horizontal animated">
                            報名參加開幕論壇
                        </md-button> -->
                        <md-button @click="goTO_ID( 'section-result' )"
                                   class="md-rose md-lg block-text faa-horizontal animated">
                            活動成果
                        </md-button>
                    </div>
                </div>
            </div>
        </parallax>

        <div class="main main-raised">

            <Details></Details>

            <Schedule class="bg-coopathon" :style="classStyle.bgCoopathon"></Schedule>

            <Rules></Rules>

            <Ideas class="bg-coopathon-2" :style="classStyle.bgCoopathon2"></Ideas>

            <Prizes></Prizes>

            <Book class="bg-coopathon-2" :style="classStyle.bgCoopathon2"></Book>

            <Result></Result>

            <Contact class="bg-coopathon-3" :style="classStyle.bgCoopathon3"></Contact>

        </div>

    </div>
</template>

<script>
    import Details from '@/views/sections/Details'
    import Schedule from '@/views/sections/Schedule'
    import Rules from '@/views/sections/Rules'
    import Ideas from '@/views/sections/Ideas'
    import Prizes from '@/views/sections/Prizes'
    import Book from '@/views/sections/Book'
    import Result from '@/views/sections/Result'
    import Contact from '@/views/sections/Contact'

    export default {
        bodyClass: "landing-page",
        components: {
            Details,
            Schedule,
            Rules,
            Ideas,
            Prizes,
            Book,
            Result,
            Contact,
        },
        props: {
            header: {
                type: String,
                default: require("@/assets/img/bg_landing.jpg")
            },
            teamImg1: {
                type: String,
                default: require("@/assets/img/faces/avatar.jpg")
            },
            teamImg2: {
                type: String,
                default: require("@/assets/img/faces/christian.jpg")
            },
            teamImg3: {
                type: String,
                default: require("@/assets/img/faces/kendall.jpg")
            }
        },
        data() {
            return {
                name: null,
                email: null,
                message: null,
                classStyle: {
                    bgCoopathon:
                    {
                        backgroundImage: 'url(' + process.env.BASE_URL + 'img/bg.jpg)',
                    },
                    bgCoopathon2:
                    {
                        backgroundImage: 'url(' + process.env.BASE_URL + 'img/bg-2.jpg)',
                    },
                    bgCoopathon3:
                    {
                        backgroundImage: 'url(' + process.env.BASE_URL + 'img/bg-3.jpg)',
                    },
                },
            };
        },
        computed: {
            headerStyle() {
                return {
                    backgroundImage: `url(${this.header})`
                };
            }
        },
        methods: {

            goTO_ID (divID) {
                let target = document.getElementById( divID )

                target.scrollIntoView({
                    block: "start",
                    behavior: "smooth"
                });
            },

            getImgURL (img)
            {
                return process.env.BASE_URL + img
            },
        }
    };
</script>

<style lang="scss" scoped>

    .container
    {
        margin-top: 50px;
    }

    .md-card-actions.text-center {
        display: flex;
        justify-content: center !important;
    }

    .contact-form {
        margin-top: 30px;
    }

    .md-has-textarea+.md-layout {
        margin-top: 15px;
    }
</style>