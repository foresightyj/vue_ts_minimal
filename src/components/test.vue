<template>
  <span>HI</span>
</template>

<script lang="ts">
import Vue from "vue";
import { Prop } from "vue/types/options";
export default Vue.extend({
  props: {
    TestId: {
      require: true,
      type: Number as Prop<number>
    }
  },
  data() {
    return {
      showDialog: false
    };
  },
  methods: {
    handleSelectionChange(): void {
      console.log(this.showDialog);
    }
  }
});
</script>
