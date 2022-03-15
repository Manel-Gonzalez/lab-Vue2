<template>
  <div class="body-container">
    <div  class="card-container" v-for="post in posts" v-bind:key="post">
      {{post.title}}
      {{post.description}}
      {{post.content}}
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
   data(){
    return{
      posts:[
        {
          title:"lamama1",
          description:"delamama1",
          content:"delamamadelamamadelamamadelamamadelamamadelamamadelamamadelamamadelamama"
        },
        {
          title:"lamama2",
          description:"delamama2",
          content:"delamamadelamamadelamamadelamamadelamamadelamamadelamamadelamamadelamama"
        },
        {
          title:"lamama3",
          description:"delamama3",
          content:"delamamadelamamadelamamadelamamadelamamadelamamadelamamadelamamadelamama"
        }
      ]
    }
  },

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
