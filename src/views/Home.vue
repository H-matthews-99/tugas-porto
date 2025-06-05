<template>
  <div class="home-container">
    <img :src="foto" alt="Foto Saya" class="profile-pic" />
    <h1>Halo, Saya Iqmal Hidayat Sormin</h1>
    <p>Mahasiswa UIR Jurusan Teknik Informatika</p>
  </div>
</template>

<script>
import foto from '@/assets/foto.jpg'

export default {
  data() {
    return {
      foto
    }
  }
}
</script>

<style scoped>
.home-container {
  text-align: center;
  margin-top: 50px;
  padding: 20px;
}

.profile-pic {
  width: 180px;
  height: 180px;
  border-radius: 50%;
  object-fit: cover;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
  margin-bottom: 20px;
}
</style>
