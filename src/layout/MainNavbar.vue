<template>
    <div>
        
        <md-toolbar id="toolbar" md-elevation="0" class="md-transparent md-absolute" :class="extraNavClasses"
            :color-on-scroll="colorOnScroll">
            <div class="md-toolbar-row md-collapse-lateral">
                <div class="md-toolbar-section-start">
                    <h3 class="md-title clickable scrollactive-item" @click="go_home">2019 食農合作松</h3>
                </div>
                <div class="md-toolbar-section-end">
                    <md-button class="md-just-icon md-simple md-toolbar-toggle" :class="{ toggled: toggledClass }"
                        @click="toggleNavbarMobile()">
                        <span class="icon-bar"></span>
                        <span class="icon-bar"></span>
                        <span class="icon-bar"></span>
                    </md-button>

                    

                    

                    <div class="md-collapse">
                        <div class="md-collapse-wrapper">
                            <mobile-menu nav-mobile-section-start="false">
                                <!-- Here you can add your items from the section-start of your toolbar -->
                            </mobile-menu>

                            <md-list>

                                <md-list-item id="main-nav">
                                    <md-list>
                                        <scrollactive
                                            class="header-nav"
                                            active-class="active"
                                            :offset="100"
                                            :duration="800"
                                            bezier-easing-value=".5,0,.35,1"
                                            :modifyUrl="false"
                                        >
                                            <md-list-item>
                                            <a href="#section-details" class="scrollactive-item">
                                                    <!-- <i class="material-icons">content_paste</i> -->
                                                    <p>關於</p>
                                                </a>
                                            </md-list-item>
                                            <md-list-item>
                                                <a href="#section-schedule" class="scrollactive-item" >
                                                    <!-- <i class="material-icons">content_paste</i> -->
                                                    <p>活動時程</p>
                                                </a>
                                            </md-list-item>
                                            <md-list-item>
                                                <a href="#section-rules" class="scrollactive-item">
                                                    <!-- <i class="material-icons">content_paste</i> -->
                                                    <p>競賽規則</p>
                                                </a>
                                            </md-list-item>
                                            <md-list-item>
                                                <a href="#section-ideas" class="scrollactive-item">
                                                    <!-- <i class="material-icons">content_paste</i> -->
                                                    <p>主題發想</p>
                                                </a>
                                            </md-list-item>
                                            <md-list-item>
                                                <a href="#section-prizes" class="scrollactive-item">
                                                    <!-- <i class="material-icons">content_paste</i> -->
                                                    <p>獎勵方式</p>
                                                </a>
                                            </md-list-item>
                                            <md-list-item>
                                                <a href="#section-contact" class="scrollactive-item">
                                                    <!-- <i class="material-icons">content_paste</i> -->
                                                    <p>辦理單位</p>
                                                </a>
                                            </md-list-item>
                                        </scrollactive>

                                    </md-list>
                                </md-list-item>
                                
                                

                                <!-- <md-list-item href="https://demos.creative-tim.com/vue-material-kit/documentation/"
                                    target="_blank" v-if="showDownload">
                                    <i class="material-icons">content_paste</i>
                                    <p>Documentation</p>
                                </md-list-item>

                                <md-list-item href="javascript:void(0)" @click="scrollToElement()" v-if="showDownload">
                                    <i class="material-icons">cloud_download</i>
                                    <p>Download</p>
                                </md-list-item>
                                <li class="md-list-item" v-else>
                                    <a href="javascript:void(0)"
                                        class="md-list-item-router md-list-item-container md-button-clean dropdown">
                                        <div class="md-list-item-content">
                                            <drop-down direction="down">
                                                <md-button slot="title"
                                                    class="md-button md-button-link md-white md-simple dropdown-toggle"
                                                    data-toggle="dropdown">
                                                    <i class="material-icons">view_carousel</i>
                                                    <p>Examples</p>
                                                </md-button>
                                                <ul class="dropdown-menu dropdown-with-icons">
                                                    <li>
                                                        <a href="#/landing">
                                                            <i class="material-icons">view_day</i>
                                                            <p>Landing Page</p>
                                                        </a>
                                                    </li>
                                                    <li>
                                                        <a href="#/login">
                                                            <i class="material-icons">fingerprint</i>
                                                            <p>Login Page</p>
                                                        </a>
                                                    </li>
                                                    <li>
                                                        <a href="#/profile">
                                                            <i class="material-icons">account_circle</i>
                                                            <p>Profile Page</p>
                                                        </a>
                                                    </li>
                                                </ul>
                                            </drop-down>
                                        </div>
                                    </a>
                                </li> -->

                                <!-- <md-list-item href="https://twitter.com/CreativeTim" target="_blank">
                                    <i class="fab fa-twitter"></i>
                                    <p class="hidden-lg">Twitter</p>
                                    <md-tooltip md-direction="bottom">Follow us on Twitter</md-tooltip>
                                </md-list-item>
                                <md-list-item href="https://www.facebook.com/CreativeTim" target="_blank">
                                    <i class="fab fa-facebook-square"></i>
                                    <p class="hidden-lg">Facebook</p>
                                    <md-tooltip md-direction="bottom">Like us on Facebook</md-tooltip>
                                </md-list-item>
                                <md-list-item href="https://www.instagram.com/CreativeTimOfficial" target="_blank">
                                    <i class="fab fa-instagram"></i>
                                    <p class="hidden-lg">Instagram</p>
                                    <md-tooltip md-direction="bottom">Follow us on Instagram</md-tooltip>
                                </md-list-item> -->

                            </md-list>
                        </div>
                    </div>
                </div>
            </div>
        </md-toolbar>
    </div>
</template>

<script>
    let resizeTimeout;

    function resizeThrottler(actualResizeHandler) {
        // ignore resize events as long as an actualResizeHandler execution is in the queue
        if (!resizeTimeout) {
            resizeTimeout = setTimeout(() => {
                resizeTimeout = null;
                actualResizeHandler();

                // The actualResizeHandler will execute at a rate of 15fps
            }, 66);
        }
    }

    import MobileMenu from "@/layout/MobileMenu";
    export default {
        components: {
            MobileMenu
        },
        props: {
            type: {
                type: String,
                default: "white",
                validator(value) {
                    return [
                        "white",
                        "default",
                        "primary",
                        "danger",
                        "success",
                        "warning",
                        "info"
                    ].includes(value);
                }
            },
            colorOnScroll: {
                type: Number,
                default: 0
            }
        },
        data() {
            return {
                extraNavClasses: "",
                toggledClass: false,
            };
        },
        computed: {
            showDownload() {
                const excludedRoutes = ["login", "landing", "profile"];
                return excludedRoutes.every(r => r !== this.$route.name);
            }
        },
        watch: {
        },
        methods: {

            go_home () {
                let body = document.body; // For Safari
                let html = document.documentElement; // Chrome, Firefox, IE and Opera places the overflow at the html level, unless else is specified. Therefore, we use the documentElement property for these browsers
                
                body.scrollIntoView({
                    block: "start",
                    behavior: "smooth"
                });
                html.scrollIntoView({
                    block: "start",
                    behavior: "smooth"
                });
            },

            bodyClick() {
                let bodyClick = document.getElementById("bodyClick");

                if (bodyClick === null) {
                    let body = document.querySelector("body");
                    let elem = document.createElement("div");
                    elem.setAttribute("id", "bodyClick");
                    body.appendChild(elem);

                    let bodyClick = document.getElementById("bodyClick");
                    bodyClick.addEventListener("click", this.toggleNavbarMobile);
                } else {
                    bodyClick.remove();
                }
            },
            toggleNavbarMobile() {
                this.NavbarStore.showNavbar = !this.NavbarStore.showNavbar;
                this.toggledClass = !this.toggledClass;
                this.bodyClick();
            },
            handleScroll() {
                let scrollValue =
                    document.body.scrollTop || document.documentElement.scrollTop;
                let navbarColor = document.getElementById("toolbar");
                this.currentScrollValue = scrollValue;
                if (this.colorOnScroll > 0 && scrollValue > this.colorOnScroll) {
                    this.extraNavClasses = `md-${this.type}`;
                    navbarColor.classList.remove("md-transparent");
                } else {
                    if (this.extraNavClasses) {
                        this.extraNavClasses = "";
                        navbarColor.classList.add("md-transparent");
                    }
                }
            },
            scrollListener() {
                resizeThrottler(this.handleScroll);
            },
            scrollToElement( el_ID) {
                let element_id = document.getElementById( el_ID );
                if (element_id) {
                    element_id.scrollIntoView({
                        block: "start",
                        behavior: "smooth"
                    });
                }
            },

        },
        mounted() {
            document.addEventListener("scroll", this.scrollListener);
        },
        beforeDestroy() {
            document.removeEventListener("scroll", this.scrollListener);
        }
    };
    
</script>

<style lang="scss" scoped>

#main-nav
{
    width:50vw;
    @media screen and (max-width: 970px)
    {
        width: 98vw !important;
    }

    .md-list-item-default
    {
        width: 95%;
        text-align: center;
        
        p
        {
            margin-bottom: 0px;
        }
    }
    ul.md-list
    {
        width: 100%;
    }
}

.header-nav.scrollactive-nav
{
    width: 100%;
    text-align: center;

    @media screen and (min-width: 970px)
    {
        .md-list-item
        {
            display: inline-block;
        }
    }

    .scrollactive-item
    {
        p
        {
            font-size: 1.0rem !important;
        }
        
        &:hover
        {
            color: #da7070 !important;
        }
    }
    .scrollactive-item.active
    {
        color: #54c4c6 !important;
    }
}

</style>