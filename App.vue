<!-- <template>
  
  <div id="app">
     <BookForm ref="bookForm" @save-book="addOrEditBook" /> 
    <BookList
      :books="books"
      @edit-book="editSelectedBook"
      @delete-book="deleteSelectedBook"
    />
  </div>
</template>

<script>
import BookForm from "./components/book/BookForm.vue";
import BookList from "./components/book/BookList.vue";

export default {
  // name: "App",
  components: {
    BookForm,
    BookList,
  },
  data() {
    return {
      books: [{ id: 1, name: "vuejs", author: "陈恒", publisher: "清华大学" }],
      selectedBookIndex: null,
      isEditing: false,
    };
  },
  methods: {
    addOrEditBook(book) {
      if (this.isEditing) {
        // 如果是在编辑状态，更新选中的书籍信息
        this.books[this.selectedBookIndex] = book;
        this.isEditing = false;
      } else {
        // 如果是添加新书，直接添加到列表
        this.books.push(book);
      }
      this.$refs.bookForm.book = {
        name: "",
        author: "",
        publisher: "",
      };
    },
    editSelectedBook(index) {
      this.selectedBookIndex = index;
      this.isEditing = true;
      const selectedBook = this.books[index];
      this.$refs.bookForm.book = {
        name: selectedBook.name,
        author: selectedBook.author,
        publisher: selectedBook.publisher,
      };
    },
    deleteSelectedBook(index) {
      this.books.splice(index, 1);
    },
  },
};
</script>

<style>

table,
th,
td {
    border: 1px solid black;
}
</style> -->

<script setup>
import abc from './components/pinia/Login.vue'
</script>

<template>

    <abc></abc>

</template>