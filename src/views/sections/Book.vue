<template>
    
    <div id="section-book" class="section">
        <div class="container">
            <div class="md-layout">
                <div class="md-layout-item md-size-80 md-xsmall-size-100 mx-auto">
                    <h2 class="text-center title">活動手冊</h2>
                </div>
            </div>

            <b-row class="justify-content-center">
                <b-col cols=11 md=8>
                    <div class="pdf-viewer">
                        <!-- <iframe :src="getBookURL" frameborder="0" height="500px" width="100%"></iframe> -->
                        <object :data="getBookURL" type="application/pdf" width="100%">
                            <embed :src="getBookURL" type="application/pdf" />
                        </object>
                    </div>
                </b-col>
            </b-row>
            


        </div>
    </div>

</template>

<script>
export default {
    data () {
        return {
            url_book: './files/2019.11.16-17 食農合作松_活動手冊.pdf',
        }
    },
    computed: {

        getBookURL ()
        {
            console.log( location )
            return location + this.url_book// + '&embedded=true'
        },

    },
}
</script>

<style lang="scss" scoped>

.pdf-viewer object
{
    height: 800px;
}


</style>