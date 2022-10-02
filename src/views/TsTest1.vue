<template>
  <div class="home" style="display: flex; justify-content: center">
    <div style="display: flex; align-items: center">
      <button @click="subtract">-</button>
      <div>{{ count }}</div>
      <button @click="add">+</button>
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue"

export default defineComponent({
  name: "TsTest1",
  data() {
    return {
      count: 0
    }
  },
  methods: {
    subtract() {
      this.count -= 1
    },
    add() {
      this.count += 1
    }
  }
})
</script>
<style lang="scss" scoped></style>
