<template>
  <div>
    <h1>Proyek Saya</h1>
    <ul>
      <li v-for="project in projects" :key="project.id">
        <h3>{{ project.title }}</h3>
        <p>{{ project.description }}</p>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        { id: 1, title: "Website Toko Online", description: "Vue + Firebase" },
        { id: 2, title: "Aplikasi To-Do", description: "Vue + Vuex" },
      ]
    }
  }
}
</script>
