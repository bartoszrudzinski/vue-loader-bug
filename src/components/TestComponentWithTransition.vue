<template>
  <TransitionComponent>
    <!-- Remove the comment so that content can be rendered at all -->
    <div v-if="isVisible">Test component with transition</div>
    <section v-else>Loading...</section>
  </TransitionComponent>
</template>

<script>
import TransitionComponent from "@/components/TransitionComponent";

export default {
  name: "TestComponentWithTransition",
  components: { TransitionComponent },
  data() {
    return {
      isVisible: false,
    };
  },
  mounted() {
    setTimeout(() => {
      this.isVisible = true;
    }, 1000);
  },
};
</script>
