<template>
  <h1>Job Details</h1>
  <p>The job id is {{id}}</p>
</template>

<script>
export default {
  name: "JobDetailsView",
  created() {},
  data() {
    return {
      id: this.$route.params.id,
    };
  },
  props: {},
  methods: {},
};
</script>

<style lang="scss" scoped></style>