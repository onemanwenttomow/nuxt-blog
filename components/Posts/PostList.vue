<template lang="html">
    <section class="post-list">
        <PostPreview
            id="1"
            thumbnail = "https://loremflickr.com/320/240"
            title= "Hello there!"
            previewText = "This is my first post"
        />
        <PostPreview
            id="2"
            thumbnail = "https://loremflickr.com/320/240"
            title= "Hello there 2!"
            previewText = "This is my first post"
        />
        <PostPreview
            id="3"
            thumbnail = "https://loremflickr.com/320/240"
            title= "Hello there! 3"
            previewText = "This is my first post"
        />
    </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'

export default {
  components: {
      PostPreview
  }
}
</script>

<style lang="css" scoped>
    .posts-page {
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .post-list {
      display: flex;
      padding: 20px;
      box-sizing: border-box;
      flex-wrap: wrap;
      align-items: center;
      justify-content: center;
    }
</style>
