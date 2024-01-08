<template>
  <footer class="app-footer">{{ stats.active }} more to do, {{ stats.done }} done</footer>
</template>
<script lang="ts">
import IStats from "@/types/Stats";
import { defineComponent, PropType } from "vue";

export default defineComponent({
  props: {
    stats: {
      type: Object as PropType<IStats>,
      required: true,
    },
  },
});
</script>
