<template>
  <div class="post" v-for="post in posts">
    <div><strong>Название:</strong>{{ post.title }}</div>
    <div><strong>Описнаие:</strong>{{ post.body }}</div>
  </div>
</template>

<script>
export default {
    props: {
        posts: {
            type: Array,
            required: true
        }
    }
};
</script>

<style scoped>
.post {
  padding: 15px;
  margin-top: 15px;
  border: 2px solid teal;
}
</style>
