<template>
  <div class="book-item">
    <h1>{{ book.title }}</h1>
    <br />

    <div style="width: 100%; text-align: left">
      <img
        style="float: left; padding: 20px"
        width="200px"
        v-bind:src="book.thumbnailUrl"
      /><br />
      <div style="padding: 20px">
        <b>Author:</b> {{ book.author }} <br />
        <b>category:</b> {{ book.category }} <br />
        <b>ISBN:</b> {{ book.isbn }}<br />
        <b>Pages:</b> {{ book.pageCount }} <br />
        <b>Deacription:</b><br />
        <p>{{ book.shortDescription }}</p>
      </div>
    </div>
    <br />
  </div>
</template>



<script>
export default {
  name: "BookItem",
  components: {},
  props: ["book"],
};
</script>

<style>
.book-item {
  background: rgb(109, 139, 134);
  padding: 10px;
  border-bottom: indigo 1px;
}
</style>