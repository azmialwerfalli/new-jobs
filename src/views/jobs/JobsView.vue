<template>
  <h1>Jobs</h1>
  <div v-for="job in jobs" :key="job.id">
    <h2>{{ job.title}}</h2>
  </div>
</template>

<script>
export default {
    data() {
        return  {
            jobs: [
                {title: "a full stack Master", id:1,details:"Master Programmer that has no life"},        
                {title: "a front end Develoer", id:2,details:"just a cute child that put boxes above each other"},
                {title: "a back end developer", id:3,details:"that other child that's loud and always mad"}
            ]
        }
    }
}
</script>

<style>

</style>