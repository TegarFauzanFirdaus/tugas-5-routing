<template>
  <div class="content">
    <h2 class="hero py-4 text-center mb-4">
      <div class="teks" v-for="article in articles" :key="article.id">
        <nuxt-link
          class="title-task mb-1"
          :to="'articles/detail/' + article.id"
        >
          {{ article.title }}
        </nuxt-link>
      </div>
    </h2>
  </div>
</template>
<script>
export default {
  data() {
    return {
      articles: [
        {
          id: 1,
          title: 'Judul Artikel 1',
          content:
            'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Placeat dolor explicabo sint quos exercitationem fugiat reiciendis assumenda. Ad quia veritatis, dolor odit, voluptas numquam modi porro eius reprehenderit ullam tenetur?',
          img: 'https://images.unsplash.com/photo-1649282806617-c51bb282899c?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2070&q=80',
        },
        {
          id: 2,
          title: 'Judul Artikel 2',
          content:
            'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Placeat dolor explicabo sint quos exercitationem fugiat reiciendis assumenda. Ad quia veritatis, dolor odit, voluptas numquam modi porro eius reprehenderit ullam tenetur?',
          img: 'https://images.unsplash.com/photo-1635732646038-0a1a2fe3f2d6?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1074&q=80',
        },
        {
          id: 3,
          title: 'Judul Artikel 3',
          content:
            'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Placeat dolor explicabo sint quos exercitationem fugiat reiciendis assumenda. Ad quia veritatis, dolor odit, voluptas numquam modi porro eius reprehenderit ullam tenetur?',
          img: 'https://images.unsplash.com/photo-1640006807976-a6127e9d6fa0?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1171&q=80',
        },
      ],
    }
  },
}
</script>
<style scoped>
.teks {
  margin-bottom: 1.5%;
  text-decoration: none;
}

.title-task {
  text-decoration: none;
  /* Jika Anda ingin mengatur warna teks, Anda juga dapat menambahkan properti color */
  color: rgb(98, 97, 97); /* Ganti dengan warna yang Anda inginkan */
  padding: 0 2%;
}

.title-task:hover {
  color: rgb(34, 34, 247);
}
</style>
