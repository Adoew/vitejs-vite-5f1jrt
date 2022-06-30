<template>
  <Standard :appParameters="AppParameters" ref="standard" />
</template>
<script>
export default {
  components: {
    Standard,
  },
  methods: {
    UpdateComponent() {
      console.log(this.$refs['standard']);
    },
  },
  mounted() {
    this.UpdateComponent();
  },
  data() {
    return {
      AppParameters: null,
    };
  },
};
</script>
