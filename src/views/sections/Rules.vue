<template>
    
    <div id="section-rules" class="section">
        <div class="container">
            <div class="md-layout">
                <div class="md-layout-item md-size-80 md-xsmall-size-100 mx-auto">
                    <h2 class="text-center title">競賽規則</h2>
                    <p class="description">
                        所有對於農業合作有興趣的朋友、專業團隊以及各大專院校學生皆可組隊報名，報名以團隊方式受理，每隊人數 1 - 6 人，團隊中至少需有 1 人具備資料分析與應用或前端視覺化開發之技術或經驗。
                    </p>
                    <p class="description">
                        本次競賽分兩階段進行：初審及決賽。團隊報名時須提供<a class="emphasis" :href="url_proposal" target="_blank">「提案說明」</a>作為初審之評選依據。入選之團隊將於 16 - 17 日的決賽進行 24 小時的黑客松競賽，須依照提案針對特定食農議題，利用程式設計發展解決方案。
                    </p>
                    <p class="description">
                        參賽提案需鎖定至少一個食農相關問題，具備「合作」之精神，結合軟體與資料分析技術發展解決方案。活動過程不限開發語言，但資料成果需以 HTML 的網頁格式發表，並將競賽提案相關原始碼上傳至 GitHub。本活動歡迎偷跑，可先行構思，但禁止使用已完成並公開發表之作品參加比賽。
                    </p>
                    <p class="description">
                        我們對「合作精神」的想像，至少包括了「共享」、「共學」與「共造」等精神，也就是透過共同分享資源、結合各領域專業共同學習成長，進而打造創新的概念與社會性的產品，用集體的力量解決問題。我們也歡迎各位提出您對「合作精神」的想像，用合作創造更完整的合作。
                    </p>

                    <br>

                    <h3>參賽辦法</h3>
                    <p>
                        <ol>
                            <li>
                                不限領域、年齡，歡迎各領域專才踴躍報名。
                            </li>
                            <li>
                                免報名費，但需繳交保證金 1000 元／隊。每隊由 1 位代表報名即可。保證金將於活動現場全額退回，未全程完成競賽之隊伍者恕不退還。11 月 16 日上午舉辦之論壇為本次競賽之一部分，入選團隊須派至少1名團員參與論壇，方算全程完成活動。
                            </li>
                            <li>
                                報名參賽隊伍至<a class="emphasis" :href="url_kktix" target="_blank"> KKTIX 報名</a>並繳交保證金後，尚需完成填寫<a class="emphasis" :href="url_proposal" target="_blank">「提案說明」</a> ，並下載<a class="emphasis" :href="url_agreement" target="_blank">「參賽同意書」</a>與<a class="emphasis" :href="url_copyright" target="_blank">「作品授權書」</a>填寫掃描後存成pdf檔，回傳至 coopathon2019@gmail.com ，標題請填寫 2019 食農合作黑客松參賽同意書與授權書（團隊名稱 – 團隊代表人姓名） 才算報名完成。
                            </li>
                            <li>
                                禁止使用已完成並公開發表之作品參加比賽，若題目曾公開發表，則須於提案時清楚說明本次提案內容與先前公開版本之差異。
                            </li>
                            <li>
                                決賽日，團隊須於 17 日中午十二點前將競賽期間開發之原始碼上傳至指定的 Github，並需派人上台展示簡報及開發成果，每隊報告 6 分鐘、評審問答 6 分鐘，共計 12 分鐘。
                            </li>
                            <li>
                                參賽作品必須遵守所有法規，並以開放源始碼發佈，採用 Creative Commons 授權規則中的「署名-非商業性使用-相同方式共享」的授權許可，參賽團隊其延續作品或衍生作品則不在此限。
                            </li>
                        </ol>
                    </p>

                    <br>

                    <h3>注意事項</h3>
                    <p>
                        <ol>
                            <li>
                                報名時間自 10 月 1 日 (二) 上午 10:00 至 10 月 27 日（日）23:59 止，一律採網路報名。馬上報名！
                            </li>
                            <li>
                                現場提供餐飲茶水、網路、電力設備，現場無衛浴設備，參賽者可依個人需求攜帶所需設備，如筆電、平板、睡袋等。
                            </li>
                            <li>
                                本次活動場地無提供衛浴設備。
                            </li>
                            <li>
                                本次活動需使用中文簡報。
                            </li>
                        </ol>
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
            url_kktix: '#',
            url_proposal: 'https://reurl.cc/W4LAK9',
            url_agreement: '#',
            url_copyright: '#',
        }
    },
}
</script>

<style lang="scss" scoped>

h3 {
    margin-bottom: 20px;
}
li {
    margin-bottom: 15px;
}

</style>