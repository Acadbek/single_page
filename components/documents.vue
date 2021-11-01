<template>
  <div>
    <ul v-if="news.length">
      <li v-for="(item, index) in news" :key="index">
        <nuxt-link class="nuxtLink" :to="`/documents/${item.id}`"
          ><p class="item__name">{{ item.name }}</p>
        </nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: {
    news: {
      type: Array,
      default: () => {
        return [
          {
            name: "O'zbekiston Respublikasi Prezidenti farmoni",
            id: 1,
          },
          {
            name: "O'zbekiston Respublikasi Prezidenti farmoni",
            id: 2,
          },
          {
            name: "O'zbekiston Respublikasi Prezidenti farmoni",
            id: 3,
          },
          {
            name: "O'zbekiston Respublikasi Prezidenti farmoni",
            id: 4,
          },
          {
            name: "O'zbekiston Respublikasi Prezidenti farmoni",
            id: 5,
          },
          {
            name: "O'zbekiston Respublikasi Prezidenti farmoni",
            id: 6,
          },
          {
            name: "O'zbekiston Respublikasi Prezidenti farmoni",
            id: 7,
          },
          {
            name: "O'zbekiston Respublikasi Prezidenti farmoni",
            id: 8,
          },
          {
            name: "O'zbekiston Respublikasi Prezidenti farmoni",
            id: 9,
          },
          {
            name: "O'zbekiston Respublikasi Prezidenti farmoni",
            id: 10,
          },
          {
            name: "O'zbekiston Respublikasi Prezidenti farmoni",
            id: 11,
          },
          {
            name: "O'zbekiston Respublikasi Prezidenti farmoni",
            id: 12,
          },
          {
            name: "O'zbekiston Respublikasi Prezidenti farmoni",
            id: 13,
          },
        ]
      },
    },
  },
  mounted() {
    console.log(this.news)
  },
}
</script>

<style scoped>
.nuxtLink {
  background: rgb(104, 77, 77);
  padding: 20px;
}
</style>
