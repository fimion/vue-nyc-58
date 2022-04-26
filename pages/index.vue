<template>
  <div>
    <ul>
      <li v-for="article in articles">
        <nuxt-link :to="article.path">{{article.title}}</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  async asyncData({$content, params}) {

    const articles = await $content('article').fetch();

    return {
      articles,
    }

  }
}
</script>
