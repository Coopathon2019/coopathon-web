<template>
    
    <div id="section-schedule" class="section">
        <div class="container">
            <div class="md-layout">
                <div class="md-layout-item md-size-80 md-xsmall-size-100 mx-auto">
                    <h2 class="text-center title">活動時程</h2>
                </div>
            </div>

            <!-- TimeLine -->
            <b-row>
                <b-col md=12>
                    <div>

                        <div class="timeline">
                            <div class="timeline-container left">
                                <div class="content">
                                    <div class="content-title">食農合作松 說明會</div>
                                    <div class="content-date"><md-icon>date_range</md-icon> 2019-09-28</div>
                                    <div class="content-time">14:00-16:30</div>
                                    <p class="text-center">
                                        <md-button href="#" class="md-success md-lg" target="_blank" :disabled="true">
                                            <!-- <i class="fas fa-angle-double-right block-text"></i> -->
                                            參加說明會
                                        </md-button>
                                    </p>
                                    <p class="text-center">
                                        <md-icon>room</md-icon> 空總臺灣當代文化實驗場 服務中心-2樓工作坊
                                        <br>（ 台灣台北市臺北市大安區建國南路一段177號 ）
                                    </p>
                                </div>
                            </div>
                            <div class="timeline-container right">
                                <div class="content">
                                    <div class="content-title">食農合作松 開放報名</div>
                                    <div class="content-date"><md-icon>date_range</md-icon> 2019-10-01</div>
                                    <div class="content-time">10:00 開始</div>
                                    <p class="text-center">
                                        <md-button href="#" class="md-success md-lg" target="_blank" :disabled="false">
                                            <!-- <i class="fas fa-angle-double-right block-text"></i> -->
                                            報名參加
                                        </md-button>
                                    </p>
                                </div>
                            </div>
                            <div class="timeline-container left">
                                <div class="content">
                                    <div class="content-title">食農合作松 報名截止</div>
                                    <div class="content-date"><md-icon>date_range</md-icon> 2019-10-27</div>
                                    <div class="content-time">23:59 截止</div>
                                    <!-- <p>Lorem</p> -->
                                </div>
                            </div>
                            <div class="timeline-container right">
                                <div class="content">
                                    <div class="content-title">
                                        <div class="icon icon-warning">
                                            <md-icon class="md-size-2x">new_releases</md-icon>
                                        </div>
                                        初選公告入圍 15 組
                                    </div>
                                    <div class="content-date"><md-icon>date_range</md-icon> 2019-11-04</div>
                                    <div class="content-time">12:00</div>
                                    <p class="text-center">
                                        <md-button href="#" class="md-success md-lg" target="_blank" :disabled="true">
                                            <!-- <i class="fas fa-angle-double-right block-text"></i> -->
                                            初選入圍名單
                                        </md-button>
                                    </p>
                                </div>
                            </div>
                            <div class="timeline-container left">
                                <div class="content">
                                    <div class="content-title">食農合作松 － 啟動論壇</div>
                                    <div class="content-date"><md-icon>date_range</md-icon> 2019-11-16</div>
                                    <div class="content-time">上午</div>
                                    <p class="text-center">
                                        <md-icon>room</md-icon> 空總臺灣當代文化實驗場
                                        <br>聯合餐廳 1 樓灰盒子空間
                                        <br>（ 台北市大安區建國南路一段 177 號 ）
                                    </p>
                                </div>
                            </div>
                            <div class="timeline-container right">
                                <div class="content">
                                    <div class="content-title">
                                        <div class="icon icon-danger">
                                            <md-icon class="md-size-2x">stars</md-icon>
                                        </div>
                                        食農合作松
                                    </div>
                                    <div class="content-date"><md-icon>date_range</md-icon> 2019-11-16</div>
                                    <div class="content-time">下午</div>
                                    <div class="content-time content-connect">至</div>
                                    <div class="content-date">
                                        <!-- <md-icon>date_range</md-icon> -->
                                        2019-11-17
                                    </div>
                                    <div class="content-time">下午</div>
                                    <p class="text-center">
                                        <md-icon>room</md-icon> 空總臺灣當代文化實驗場
                                        <br>聯合餐廳 1 樓灰盒子空間
                                        <br>（ 台北市大安區建國南路一段 177 號 ）
                                    </p>
                                </div>
                            </div>
                        </div>

                    </div>
                    <!-- TimeLine END -->
                    
                </b-col>
            </b-row>
        </div>
    </div>

</template>

<script>


export default {
    
}
</script>

<style lang="scss" scoped>


/* The actual timeline (the vertical ruler) */
.timeline {
    position: relative;
    max-width: 1200px;
    margin: 0 auto;
}

/* The actual timeline (the vertical ruler) */
.timeline::after {
    content: '';
    position: absolute;
    width: 6px;
    background-color: white;
    top: 0;
    bottom: 0;
    left: 50%;
    margin-left: -3px;
}

/* timeline-Container around content */
.timeline-container {
    padding: 10px 40px;
    position: relative;
    background-color: inherit;
    width: 50%;
}

/* The circles on the timeline */
.timeline-container::after {
    content: '';
    position: absolute;
    width: 25px;
    height: 25px;
    right: -17px;
    background-color: white;
    border: 4px solid #FF9F55;
    top: 15px;
    border-radius: 50%;
    z-index: 1;
}

/* Place the timeline-container to the left */
.left {
    left: -5px;
}

/* Place the timeline-container to the right */
.right {
    left: 50%;
}

/* Add arrows to the left timeline-container (pointing right) */
.left::before {
    content: " ";
    height: 0;
    position: absolute;
    top: 22px;
    width: 0;
    z-index: 1;
    right: 30px;
    border: medium solid white;
    border-width: 10px 0 10px 10px;
    border-color: transparent transparent transparent white;
}

/* Add arrows to the right timeline-container (pointing left) */
.right::before {
    content: " ";
    height: 0;
    position: absolute;
    top: 22px;
    width: 0;
    z-index: 1;
    left: 30px;
    border: medium solid white;
    border-width: 10px 10px 10px 0;
    border-color: transparent white transparent transparent;
}

/* Fix the circle for timeline-containers on the right side */
.right::after {
    left: -13px;
}

/* The actual content */
.content {
    padding: 20px 30px;
    background-color: white;
    position: relative;
    border-radius: 6px;
    text-align: center;

    &:hover
    {
        //   cursor: pointer;
        box-shadow: 5px 5px 30px rgb(157, 157, 157);
    }

}
.content-date,
.content-date i
{
    display: inline-block;
    font-size: 1.3rem;
    font-weight: 500;
    color: #794d68;
    margin: 5px 5px 10px 0px;
}
.content-date
{
    margin-right: 15px;
}
.content-time
{
    display: inline-block;
    font-size: 1.2rem;
    font-weight: 500;
    color: #b84072;
}
.content-connect
{
    padding: 0px 10px;
}
.content-title
{
    font-size: 1.8rem;
    font-weight: 400;
    margin: 20px 0px;
    line-height: 1.8rem;

    .icon
    {
        margin-bottom: 20px;
    }
}

/* Media queries - Responsive timeline on screens less than 768px wide */
@media screen and (max-width: 768px) {

    .timeline
    {
        margin-left: -20px;
    }

    /* Place the timelime to the left */
    .timeline::after {
        left: 31px;
    }
    
    /* Full-width timeline-containers */
    .timeline-container {
        width: 100%;
        padding-left: 70px;
        padding-right: 25px;
    }
    
    /* Make sure that all arrows are pointing leftwards */
    .timeline-container::before {
        left: 60px;
        border: medium solid white;
        border-width: 10px 10px 10px 0;
        border-color: transparent white transparent transparent;
    }

    /* Make sure all circles are at the same spot */
    .left
    {
        left: 0px;
    }
    .left::after, .right::after {
        left: 18px;
    }
    
    /* Make all right timeline-containers behave like the left ones */
    .right {
        left: 0%;
    }

    .timeline-container
    {
        padding-left: 50px;
        padding-right: 10px;
    }
    /* The actual content */
    .content
    {
        padding: 10px 20px 20px 20px;
    }
    .content-date,
    .content-date i
    {
        font-size: 1.3rem;
    }
    .content-time
    {
        font-size: 1.0rem;
    }
    .content-title
    {
        font-size: 1.5rem;
    }
}

@media screen and (max-width: 400px)
{
    /* The actual content */
    .content
    {
        padding: 10px 10px 30px 10px;
    }
}

</style>