<template>
  <h1>Jobs</h1>
  <div v-for="job in jobs" :key="job.id">
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

<style lang="scss" scoped></style>