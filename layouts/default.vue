<template>
    <div>
        <div v-if="pageLoading"> 
            <img src="" alt=""/>
        </div>
        <div class="content-wrapper">
            <Header></Header>
            <Nuxt></Nuxt>
        </div>
        <Footer></Footer>
    </div>
</template>

<script>
export default{
    name: 'DefaultLayout',
    data(){
        return{
            pageLoading: true
        }
    },
    mounted(){
        this.$nextTick(() => {
            this.pageLoading = false
        })
    }
}
</script>

<style>

</style>