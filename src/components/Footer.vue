<template>
  <div >
      <footer class="footer-container">
          <p>{{2+2}}</p>
          <p>{{leroText()}}</p>
          <p>a</p>
      </footer>
  </div>
</template>

<script>
export default {
    name:"footer",
    data(){
        return{
            text:"lamamadelamamadelamamadelamama"
        }
    },
    methods:{
        leroText(){
            return this.text
            
        }
    }
}
</script>

<style>

</style>