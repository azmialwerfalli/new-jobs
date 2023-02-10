<template>
  <h1>{{job.title}}</h1>
  <p>The Job id is {{id}}</p>
  <p>{{job.details}}</p>
</template>

<script>
export default {
    props: ['id'],
    data(){
        return{
            job:null
        }
    },
    mounted() {
      fetch('http://localhost:3000/jobs/' + this.id)
      .then((res) => res.json())
      .then(data => this.jobs = data)
      .catch(err => console.log(err.message))
    }
}
</script>

<style>

</style>import 