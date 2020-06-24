<template>
  <div>
    <main>
      <b-container>
        <b-row>
          <b-col md="12">
            <ul>
              <li v-for="post in posts" :key="post.slug">
                <nuxt-link
                  :to="{ name: 'posts-id', params: { id: post.slug } }"
                  >{{ post.title }}</nuxt-link
                >
              </li>
            </ul>
          </b-col>
        </b-row>
      </b-container>
    </main>
  </div>
</template>

<script>
export default {
  data() {
    return {
      posts: []
    };
  },
  async asyncData() {
    return {
      posts: [
        {
          title: "Article 1",
          slug: "article-1"
        },
        {
          title: "Article 2",
          slug: "article-2"
        }
      ]
    };
  }
};
</script>

<style scoped></style>
