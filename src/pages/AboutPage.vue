```vue
<template>
  <div class="page">
    <!-- Judul atas -->
    <div class="top-title">
      <h3>SMK Yadika Soreang — Onlineshop</h3>

      <div class="links">
        <a href="#">Landing</a>
        <a href="#">Product</a>
        <a href="#">About</a>
        <a href="#">Contact</a>
      </div>
    </div>

    <!-- HERO -->
    <section class="hero">
      <div class="hero-content">
        <h1>
          Belanja Perlengkapan Sekolah,
          <br />
          Mudah & Terpercaya
        </h1>
        x
        <p>
          Dari buku, alat tulis hingga kebutuhan sekolah lainnya — semuanya ada
          di satu tempat.
        </p>

        <button @click="$router.push('/product')">Lihat Produk</button>
      </div>
    </section>

    <!-- KEUNGGULAN -->
    <section class="features">
      <!-- Kartu 1 -->
      <div class="feature-card">
        <div class="icon">✓</div>

        <h2>Kualitas Terjamin</h2>

        <p>Produk pilihan dengan kualitas terbaik untuk kebutuhan sekolah.</p>
      </div>

      <!-- Kartu 2 -->
      <div class="feature-card">
        <div class="icon">$</div>

        <h2>Harga Bersahabat</h2>

        <p>Harga ramah pelajar dengan produk yang tetap berkualitas.</p>
      </div>

      <!-- Kartu 3 -->
      <div class="feature-card center-card">
        <div class="icon">▣</div>

        <h2>Ambil di Sekolah</h2>

        <p>Tidak perlu jauh-jauh, pesan lalu ambil langsung di sekolah.</p>
      </div>
    </section>
  </div>
</template>

<style scoped>
* {
  box-sizing: border-box;
}

.page {
  min-height: 100vh;
  background: #f5f8fc;
  padding-bottom: 80px;
}

/* =========================
   JUDUL ATAS
========================= */

.top-title {
  width: 80%;
  margin: 0 auto;
  padding: 15px 0 8px;

  color: #333;
}

.top-title h3 {
  font-size: 15px;
  font-weight: 600;
  margin-bottom: 3px;
}

.links {
  display: flex;
  gap: 10px;
}

.links a {
  color: #0f766e;
  font-size: 13px;
  text-decoration: underline;
}

/* =========================
   HERO
========================= */

.hero {
  width: 80%;
  height: 350px;

  margin: 0 auto;

  display: flex;
  justify-content: center;
  align-items: center;

  text-align: center;

  border-radius: 0 0 8px 8px;

  background: linear-gradient(135deg, #0f766e, #0891b2, #2563eb);

  box-shadow: 0 8px 25px rgba(15, 118, 110, 0.25);
}

.hero-content {
  width: 800px;
  padding: 20px;
}

.hero h1 {
  color: white;

  font-size: 38px;
  line-height: 1.2;

  margin-bottom: 18px;

  font-weight: 700;
}

.hero p {
  color: #dffafa;

  font-size: 16px;
  line-height: 1.5;

  margin-bottom: 28px;
}

.hero button {
  border: none;

  background: white;
  color: #0f766e;

  padding: 12px 30px;

  border-radius: 25px;

  font-size: 15px;
  font-weight: bold;

  cursor: pointer;

  transition: 0.3s;
}

.hero button:hover {
  transform: translateY(-3px);

  box-shadow: 0 7px 15px rgba(0, 0, 0, 0.2);
}

/* =========================
   FEATURES
========================= */

.features {
  width: 650px;

  margin: 45px auto 0;

  display: flex;
  flex-wrap: wrap;

  justify-content: center;

  gap: 20px;
}

.feature-card {
  width: 300px;
  min-height: 150px;

  padding: 22px;

  text-align: center;

  background: white;

  border-radius: 4px;

  box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);

  transition: 0.3s;
}

.feature-card:hover {
  transform: translateY(-5px);

  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.12);
}

.icon {
  font-size: 27px;

  color: #0f766e;

  margin-bottom: 8px;

  font-weight: bold;
}

.feature-card h2 {
  font-size: 18px;

  color: #333;

  margin-bottom: 8px;
}

.feature-card p {
  color: #999;

  font-size: 13px;

  line-height: 1.4;

  margin: 0;
}

/* Kartu ketiga berada di tengah */

.center-card {
  margin-top: -2px;
}

/* =========================
   RESPONSIVE
========================= */

@media (max-width: 800px) {
  .top-title,
  .hero {
    width: 92%;
  }

  .hero {
    height: 320px;
  }

  .hero h1 {
    font-size: 30px;
  }

  .features {
    width: 92%;
  }
}

@media (max-width: 650px) {
  .features {
    flex-direction: column;
    align-items: center;
  }

  .feature-card {
    width: 90%;
  }

  .hero p {
    font-size: 14px;
  }
}
</style>
```
