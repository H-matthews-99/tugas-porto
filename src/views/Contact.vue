<template>
  <div>
    <h1>Kontak</h1>
    <form @submit.prevent="submitForm">
      <input v-model="name" placeholder="Nama" required />
      <input v-model="email" type="email" placeholder="Email" required />
      <textarea v-model="message" placeholder="Pesan" required></textarea>
      <button type="submit">Kirim</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "",
      email: "",
      message: ""
    };
  },
  methods: {
    submitForm() {
      alert(`Pesan dari ${this.name} dikirim!`);
      // Bisa dihubungkan ke API/email service
    }
  }
}
</script>
