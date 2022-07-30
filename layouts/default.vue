<template>
    <div>
        <div v-if="pageLoading" class="loader-container"> 
            <img class="img-fluid center" src="/images/logo.png" alt=""/>
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
.loader-container{
    width:100%;
    height:100%;
    text-align:center;
    line-height:100vh;
}
.center{
    width:30%;
    animation:stretch 1.5s ease-out 0s infinite alternate none running;
}

@keyframes stretch {
  0%{
    transform: scale(0.3);
  }
  100%{
    transform: scale(1);
  }
}

</style>