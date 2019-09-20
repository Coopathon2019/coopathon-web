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
                        <md-button href="https://www.accupass.com/event/1909170301505585368800" class="md-success md-lg block-text" target="_blank">
                            <!-- <i class="fas fa-angle-double-right"></i> -->
                            參加說明會
                        </md-button>
                    </div>
                </div>
            </div>
        </parallax>

        <div class="main main-raised">

            <Details></Details>

            <Schedule class="bg-linear-purple"></Schedule>

            <Rules></Rules>

            <Ideas class="bg-linear-green"></Ideas>

            <Prizes></Prizes>

            <Contact class="bg-linear-blue"></Contact>

        </div>

    </div>
</template>

<script>
    import Details from '@/views/sections/Details'
    import Schedule from '@/views/sections/Schedule'
    import Rules from '@/views/sections/Rules'
    import Ideas from '@/views/sections/Ideas'
    import Prizes from '@/views/sections/Prizes'
    import Contact from '@/views/sections/Contact'

    export default {
        bodyClass: "landing-page",
        components: {
            Details,
            Schedule,
            Rules,
            Ideas,
            Prizes,
            Contact,
        },
        props: {
            header: {
                type: String,
                default: require("@/assets/img/bg7.jpg")
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
                message: null
            };
        },
        computed: {
            headerStyle() {
                return {
                    backgroundImage: `url(${this.header})`
                };
            }
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