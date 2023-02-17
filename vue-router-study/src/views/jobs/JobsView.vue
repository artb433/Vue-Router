<template>
  <h1>Jobs</h1>
  <div v-for="job in jobs" :key="job.id">
    <h2>{{job.title}}</h2>
  </div>
</template>

<script>
export default {
  name: "Jobs",
  created() {},
  data() {
    return {
      jobs: [
        {title: "UX Designer", id:1, description: "Job 1 description"},
        {title: "Web Developer", id:2, description: "Job 2 description"},
        {title: "Mobile App Develope", id:3, description: "Job 3 description"},
      ],
    };
  },
  props: {},
  methods: {},
};
</script>

<style lang="scss" scoped></style>