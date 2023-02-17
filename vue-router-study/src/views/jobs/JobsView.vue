<template>
  <h1>Jobs</h1>
  <div v-for="job in jobs" :key="job.id" class="job">
    <router-link :to="{name: 'jobDetails', params: { id: job.id}}">
      <h2>{{job.title}}</h2>
    </router-link>
  </div>
</template>

<script>
export default {
  name: "JobsView",
  data() {
    return {
      jobs: [
        {title: "UX Designer", id:1, description: "Job 1 description"},
        {title: "Web Developer", id:2, description: "Job 2 description"},
        {title: "Mobile App Developer", id:3, description: "Job 3 description"},
      ],
    };
  },
};
</script>

<style scoped>
  .job h2{
    background: #f4f4f4;
    padding: 20px;
    border-radius: 10px;
    margin: 10px auto;
    max-width: 600px;
    cursor: pointer;
    color: #444;
  }
  .job h2:hover{
    background: #ddd;
  }
  .job a{
    text-decoration: none;
    color: #444;
  }
</style>