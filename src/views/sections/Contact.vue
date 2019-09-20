<template>
    
    <div id="section-contact" class="section">
        <div class="container">
            <div class="md-layout">
                <div class="md-layout-item md-size-80 md-xsmall-size-100 mx-auto">
                    <h2 class="text-center title">辦理單位</h2>
                    <!-- <p class="description">
                        Divide details about your product or agency work into parts.
                        Write a few lines about each one and contact us about any
                        further collaboration. We will responde get back to you in a
                        couple of hours.
                    </p> -->
                    
                </div>
            </div>

            <b-container>
                <b-row align-v="center" align-h="center" class="unit-area">
                    <b-col cols=12 md=4>
                        <h3>指導單位</h3>
                        <h4 class="unit-title">文化部</h4>
                    </b-col>
                    <b-col cols=12 md=4>
                        <a href="https://www.moc.gov.tw/" target="_blank">
                            <b-img src="./img/logo/logo_ministry_of_culture.png" alt="文化部"/>
                        </a>
                    </b-col>
                </b-row>
                <b-row align-v="center" align-h="center" class="unit-area">
                    <b-col cols=12 md=4>
                        <h3>主辦單位</h3>
                        <h4 class="unit-title">空總臺灣當代文化實驗場</h4>
                    </b-col>
                    <b-col cols=12 md=4>
                        <a href="https://clab.org.tw/" target="_blank">
                            <b-img src="./img/logo/logo_clab.png" alt="空總臺灣當代文化實驗場"/>
                        </a>
                    </b-col>
                </b-row>
                <b-row align-v="center" align-h="center" class="unit-area">
                    <b-col cols=12 md=4>
                        <h3>承辦單位</h3>
                        <h4 class="unit-title">蜂巢數據科技股份有限公司</h4>
                    </b-col>
                    <b-col cols=12 md=4>
                        <a href="https://www.beehivedt.com/" target="_blank">
                            <b-img src="./img/logo/logo_beehive_white.png" alt="蜂巢數據科技股份有限公司"/>
                        </a>
                    </b-col>
                </b-row>
            </b-container>


            <div class="md-layout">
                <div class="md-layout-item md-size-66 md-xsmall-size-100 mx-auto">
                    
                    <br>

                    <h2 class="text-center title">活動聯絡</h2>
                    <p>

                        <b-table stacked :items="contact_info"></b-table>
                        
                    </p>
                    
                </div>
            </div>


        </div>
    </div>

</template>

<script>
export default {
    data () {
        return {
            contact_info: [
                {
                    '蜂巢數據科技股份有限公司': '盧安邦　02-23679327',
                    '臺灣當代文化實驗場發展組': '郭書瑋　02 8773-5087 #303',
                    '2019 食農合作松 e-mail': 'coopathon2019@gmail.com',
                }
            ],
        }
    }
}
</script>


<style lang="scss" scoped>


.unit-area
{
    text-align: center;
    margin-top: 10px;
    margin-bottom: 15px;

    .unit-title
    {
        color: rgb(207, 251, 248);
        margin-top: 10px;
        line-height: 3.2rem;
    }

    img
    {
        // max-width: 300px;
        max-height: 60px;
    }
}

p {
    margin-bottom: 15px;
}


</style>

<style lang="scss">

    table.table th,
    table.table td
    {
        border-top: 1px solid rgba(196, 245, 242, 0.5) !important;
    }

</style>