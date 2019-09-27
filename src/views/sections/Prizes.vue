<template>
    
    <div id="section-prizes" class="section">
        <div class="container">
            <div class="md-layout">
                <div class="md-layout-item md-size-80 md-xsmall-size-100 mx-auto">
                    <h2 class="text-center title">獎勵方式</h2>
                    <!-- <h4 class="text-center description">
                        Divide details about your product or agency work into parts.
                        Write a few lines about each one and contact us about any
                        further collaboration. We will responde get back to you in a
                        couple of hours.
                    </h4> -->
                    
                </div>
            </div>

            <!-- <div class="text-center">
                <b-alert variant="success" show>
                    <h3 class="block-text">優勝 1 名</h3>
                    <h3 class="block-text">20 萬元整</h3>
                </b-alert>
                <b-alert variant="info" show>
                    <h3>優選 5 名 6 萬元整</h3>
                </b-alert>
            </div> -->

            <div class="text-center">
                <div class="md-layout">
                    <div class="md-layout-item md-medium-size-50 md-small-size-100">
                        <div class="info info-prizes">
                            <b-container>
                                <b-row class="prizes-icons" align-v="center" align-h="center">
                                    <b-col cols=12>
                                        <md-icon class="md-size-3x icon-golden">emoji_events</md-icon>
                                    </b-col>
                                </b-row>
                            </b-container>
                            <h4 class="info-title">
                                優勝 1 組
                                <div class="info-date">
                                   每組新台幣 20 萬元整，獎狀一紙
                                </div>
                            </h4>
                        </div>
                        <br>
                    </div>
                    <div class="md-layout-item md-medium-size-50 md-small-size-100" >
                        <div class="info info-prizes">
                            <b-container>
                                <b-row class="prizes-icons" align-v="center" align-h="center">
                                    <b-col cols=2>
                                        <md-icon class="md-size-2x icon-silver">emoji_events</md-icon>
                                    </b-col>
                                    <b-col cols=2>
                                        <md-icon class="md-size-2x icon-silver">emoji_events</md-icon>
                                    </b-col>
                                    <b-col cols=2>
                                        <md-icon class="md-size-2x icon-silver">emoji_events</md-icon>
                                    </b-col>
                                    <b-col cols=2>
                                        <md-icon class="md-size-2x icon-silver">emoji_events</md-icon>
                                    </b-col>
                                    <b-col cols=2>
                                        <md-icon class="md-size-2x icon-silver">emoji_events</md-icon>
                                    </b-col>
                                </b-row>
                            </b-container>
                            <h4 class="info-title">
                                優選 5 組
                                <div class="info-date">
                                    每組新台幣 6 萬元整，獎狀一紙
                                </div>
                            </h4>
                        </div>
                        <br>
                    </div>
                </div>

                <div class="md-layout">
                    <div class="md-layout-item md-size-80 md-xsmall-size-100 mx-auto">
                        <p class="description">
                            獲獎團隊應指定代表人領取獎金，由主辦單位代扣所得稅金後，將於活動結束後一個月內，匯款至團隊代表人指定帳戶。
                        </p>
                    </div>
                </div>
            </div>

            

            
            <div class="md-layout">
                <div class="md-layout-item md-size-80 md-xsmall-size-100 mx-auto">
                    <h3>
                        <div class="block-text icon icon-warning">
                            <md-icon class="md-size-2x">new_releases</md-icon>
                        </div>
                        <div class="block-text">
                            評審標準 【 初選 】
                        </div>
                    </h3>

                    <p class="description">
                        初選評選委員會由主辦單位空總臺灣當代文化實驗場邀請相關領域之外部評選委員組織而成，並依據初審評選指標（見下表）進行評選作業。
                    </p>

                    <div class="table-area">
                        <div class="table-width">
                            <b-table-simple caption-top responsive hover>
                                <!-- <caption>Items sold in August, grouped by Country and City:</caption> -->
                                <colgroup><col><col></colgroup>
                                <colgroup><col><col><col></colgroup>
                                <colgroup><col><col></colgroup>
                                <b-thead head-variant="dark">
                                    <b-tr class="text-center">
                                        <!-- <b-th>項次</b-th> -->
                                        <b-th>評選指標</b-th>
                                        <b-th>說明</b-th>
                                        <b-th>評選人員</b-th>
                                        <b-th>評分比例</b-th>
                                    </b-tr>
                                </b-thead>
                                <b-tbody>
                                    <b-tr>
                                        <!-- <b-td>1</b-td> -->
                                        <b-td>現況與問題分析</b-td>
                                        <b-td>對欲解決的問題、需求或現況是否具有足夠的理解與認識</b-td>
                                        <b-td rowspan=5 class="span-text-center">2019 食農合作松初選評委會</b-td>
                                        <b-td>20 %</b-td>
                                    </b-tr>
                                    <b-tr>
                                        <!-- <b-td>2</b-td> -->
                                        <b-td>問題解決的方式</b-td>
                                        <b-td>提出的方案是否切中問題要害，具有解決問題的潛力？</b-td>
                                        <b-td>20 %</b-td>
                                    </b-tr>
                                    <b-tr>
                                        <!-- <b-td>3</b-td> -->
                                        <b-td>跨域與創新</b-td>
                                        <b-td>提案是否結合不同領域知識與專業？內容是否打破常規，開闢創新方向？</b-td>
                                        <b-td>20 %</b-td>
                                    </b-tr>
                                    <b-tr>
                                        <!-- <b-td>4</b-td> -->
                                        <b-td>合作精神</b-td>
                                        <b-td>提案是否具備「共享」、「共學」與「共造」等合作精神？是否具有推動並擴大合作精神的潛力。</b-td>
                                        <b-td>20 %</b-td>
                                    </b-tr>
                                    <b-tr>
                                        <!-- <b-td>5</b-td> -->
                                        <b-td>提案可行性與發展潛力</b-td>
                                        <b-td>提案內容是否在現實可行範圍內並有延續、長期發展的可能性？</b-td>
                                        <b-td>20 %</b-td>
                                    </b-tr>
                                </b-tbody>
                                <!-- <b-tfoot>
                                    <b-tr>
                                        <b-td colspan="7" variant="secondary" class="text-right">
                                        Total Rows: <b>5</b>
                                        </b-td>
                                    </b-tr>
                                </b-tfoot> -->
                            </b-table-simple>
                        </div>

                    </div>

                </div>

                <div class="md-layout-item md-size-80 md-xsmall-size-100 mx-auto">
                    <h3>
                        <div class="block-text icon icon-danger">
                            <md-icon class="md-size-2x">stars</md-icon>
                        </div>
                        <div class="block-text">
                            評審標準 【 決賽 】
                        </div>
                    </h3>

                    <p class="description">
                        決賽評選委員會由主辦單位臺灣當代文化實驗場邀請關注相關領域之學界、公部門、資訊、議題社群、藝術文化等跨領域工作者組織而成，並依據決賽評選指標（見下表），進行評選作業。
                    </p>


                    <div class="table-area">
                        <div class="table-width">
                            <b-table-simple caption-top responsive hover>
                                <!-- <caption>Items sold in August, grouped by Country and City:</caption> -->
                                <colgroup><col><col></colgroup>
                                <colgroup><col><col><col></colgroup>
                                <colgroup><col><col></colgroup>
                                <b-thead head-variant="dark">
                                    <b-tr class="text-center">
                                        <!-- <b-th>項次</b-th> -->
                                        <b-th>評選指標</b-th>
                                        <b-th>說明</b-th>
                                        <b-th>評選人員</b-th>
                                        <b-th>評分比例</b-th>
                                    </b-tr>
                                </b-thead>
                                <b-tbody>
                                    <b-tr>
                                        <!-- <b-td>1</b-td> -->
                                        <b-td>現況分析與問題解決成效</b-td>
                                        <b-td>對問題現況的理解認識是否充分？完成作品是否具有解決問題的潛力？</b-td>
                                        <b-td rowspan=5 class="span-text-center">2019食農合作松決賽評委會</b-td>
                                        <b-td>20 %</b-td>
                                    </b-tr>
                                    <b-tr>
                                        <!-- <b-td>3</b-td> -->
                                        <b-td>跨域與創新</b-td>
                                        <b-td>作品是否結合不同領域知識與專業？內容是否打破常規，開闢創新方向？</b-td>
                                        <b-td>25 %</b-td>
                                    </b-tr>
                                    <b-tr>
                                        <!-- <b-td>4</b-td> -->
                                        <b-td>合作精神</b-td>
                                        <b-td>作品是否具備「共享」、「共學」與「共造」等合作精神？是否具有推動並擴大合作精神的潛力。</b-td>
                                        <b-td>25 %</b-td>
                                    </b-tr>
                                    <b-tr>
                                        <!-- <b-td>5</b-td> -->
                                        <b-td>作品完整性與發展潛力</b-td>
                                        <b-td>完成之作品是否成熟？是否具備一定程度的完整性？是否具有延續並長期發展的可能性？</b-td>
                                        <b-td>20 %</b-td>
                                    </b-tr>
                                    <b-tr>
                                        <!-- <b-td>5</b-td> -->
                                        <b-td>簡報與答詢</b-td>
                                        <b-td>團隊上台簡報成果與回應評委提問之表現。</b-td>
                                        <b-td>10 %</b-td>
                                    </b-tr>
                                </b-tbody>
                                <!-- <b-tfoot>
                                    <b-tr>
                                        <b-td colspan="7" variant="secondary" class="text-right">
                                        Total Rows: <b>5</b>
                                        </b-td>
                                    </b-tr>
                                </b-tfoot> -->
                            </b-table-simple>
                        </div>

                    </div>

                </div>
            </div>

        </div>
    </div>

</template>

<script>
export default {
    data () {
        return {
        }
    }
}
</script>

<style lang="scss" scoped>

.info-prizes
{
    padding: 35px 10px 10px 10px;
    // background-color: rgb(241, 232, 191);
    border-radius: 20px;
    border: 2px solid rgb(241, 232, 191);

    &:hover
    {
        transform: scale(1.05);
        background-color: #fdf3e8;
        box-shadow: 0 4px 8px 4px rgba(201, 157, 61, 0.2), 0 6px 20px 0 rgba(247, 180, 36, 0.19);
    }


    .prizes-icons
    {
        height: 75px;
    }
    .icon-golden
    {
        color: #e4ab40 !important;
    }
    .icon-silver
    {
        color: #888e93 !important;
    }

}

h3 .block-text
{
    vertical-align: middle;
}


.table-area
{
    overflow-x: auto;
    margin-bottom: 20px;

    .table-width,
    table
    {
        min-width: 880px;
    }

    .span-text-center
    {
        text-align: center;
        vertical-align: middle;
    }
}


</style>