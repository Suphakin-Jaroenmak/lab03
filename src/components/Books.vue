<template>
  <div>
    <div v-bind:key="book.bookid" v-for="book in book1">
      <BookItem v-bind:book="book" />
    </div>
  </div>
</template>



<script>
//import bookitem
import BookItem from "./BookItem.vue";
export default {
  name: "Books",
  components: {
    BookItem,
  },
  props: ["book1"],
};
</script>

<style>
</style>