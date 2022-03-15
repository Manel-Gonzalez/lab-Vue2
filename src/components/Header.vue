<template>
    <div >
        <header class="header-container">
            <div>
                <button @click="showButton">Apretame</button> 
                <button @click="hideImg" v-if="show">No me Apretes</button>
            </div>
            <img  v-if="showImg" class="footer-img" src="https://memegenerator.net/img/instances/74124464.jpg" alt="">
        </header>
    </div>
</template>

<script>
export default {
    name:"header",
    data(){
        return{
            show:false,
            showImg:false,
        }
    },
    methods:{
        showButton(){
            this.show = !this.show
        },
        hideImg(){
            this.showImg = !this.showImg
        }
    }
}
</script>

<style>

</style>