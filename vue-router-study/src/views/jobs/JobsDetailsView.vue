<template>
  <h1>Job Details</h1>
  <p>The job id is {{id}}</p>
</template>

<script>
export default {
  name: "JobDetailsView",
  props:['id'],
  // data() {
  //   return {
  //     id: this.$route.params.id,
  //   };
  // },
  methods: {},
};
</script>

<style lang="scss" scoped></style>