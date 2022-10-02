<template>
  <div class="home" style="display: flex; justify-content: center">
    <div style="display: flex; align-items: center">
      {{ book.title }} <br />
      {{ book.author }} <br />
      {{ book.year }}
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue"

interface Book {
  title: string
  author: string
  year: number
}

export default defineComponent({
  name: "InterFaceTest",
  data() {
    return {
      book: {
        title: "TypeScript interface Guide",
        author: "team",
        year: 2022
      } as Book
    }
  }
})
</script>
<style lang="scss" scoped></style>
