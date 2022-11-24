<template>
  <TestComponent class="extra-class" />
  <TestComponentWithTransition />
</template>

<script>
import TestComponent from "@/components/TestComponent";
import TestComponentWithTransition from "@/components/TestComponentWithTransition";

export default {
  name: "App",
  components: {
    TestComponentWithTransition,
    TestComponent,
  },
};
</script>
