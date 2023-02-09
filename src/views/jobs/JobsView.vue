<template>
  <h1>Jobs</h1>
  <div v-for="job in jobs" :key="job.id" class="job">
    <router-link :to="{name: 'JobDetails', params:{id:job.id}}">
      <h2>{{ job.title}}</h2>
    </router-link>
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
.job h2 {
  background: #f4f4f4;
  padding: 20px;
  border-radius: 10px;
  margin: 10px auto;
  max-width: 600px;
  cursor: pointer;
  color: #444;
}
.job h2:hover {
  background: #ddd;
}
.job a {
  text-decoration: none;
}
</style>