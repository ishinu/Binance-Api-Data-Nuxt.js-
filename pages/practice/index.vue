<template>
    <div>
        <section class="content text-center">
            <h1 class="display-5 mt-3">Count is : {{count}}</h1>
            <button @click='incCount' class="mt-3 btn btn-outline-success">Click here</button>
            <h3 class="mt-3">Count changed {{value}} times. </h3>
        </section>
    </div>
</template>

<script>
    export default{
        data(){
            return{
                count: 0,
                value: 0
            }
        },
        watch:{
            count(){
                this.value++
            }
        },
        methods : {
            incCount() {
                this.count++
            }
        }
    }
</script>