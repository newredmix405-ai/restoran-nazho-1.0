<head></head>
 <!DOCTYPE html>
 <html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Restoran Lezat</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0; padding: 0;
      background-color: #fafafa;
      color: #333;
    }
    header {
      background-color: #8B0000;
      color: black;
      padding: 15px 50px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    header h1 { margin: 0; }
    nav a {
      color: white;
      text-decoration: none;
      margin-left: 20px;
      font-weight: bold;
    }
    .banner {
      background: url('https://source.unsplash.com/1200x500/?food,restaurant') no-repeat center center;
      background-size: cover;
      height: 500px;
      display: flex;
      justify-content: center;
      align-items: center;
      color: white;
      text-align: center;
    }
    .banner h2 {
      font-size: 40px;
      text-shadow: 2px 2px 6px rgba(0,0,0,0.8);
    }
    .btn {
      display: inline-block;
      margin-top: 15px;
      padding: 12px 25px;
      background: #FFD700;
      color: #333;
      font-weight: bold;
      border-radius: 8px;
      text-decoration: none;
    }
    .highlight, .about, .promo, .reservasi, .order {
      padding: 50px;
      text-align: center;
    }
    .menu-items {
      display: flex;
      justify-content: center;
      gap: 30px;
      margin-top: 30px;
    }
    .menu-card {
      background: white;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0px 2px 5px rgba(0,0,0,0.1);
      width: 250px;
    }
    form {
      max-width: 500px;
      margin: auto;
      text-align: left;
      background: white;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0px 2px 5px rgba(0,0,0,0.1);
    }
    form label {
      display: block;
      margin: 10px 0 5px;
      font-weight: bold;
    }
    form input, form select, form textarea {
      width: 100%;
      padding: 10px;
      margin-bottom: 15px;
      border: 1px solid #ccc;
      border-radius: 6px;
    }
    form button {
      background: #8B0000;
      color: white;
      padding: 12px 20px;
      border: none;
      border-radius: 8px;
      font-weight: bold;
      cursor: pointer;
    }
    footer {
      background: #333;
      color: white;
      text-align: center;
      padding: 20px;
      margin-top: 30px;
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <h1>Restoran Lezat</h1>
    <nav>
      <a href="#">Home</a>
      <a href="#menu">Menu</a>
      <a href="#reservasi">Reservasi</a>
      <a href="#order">Order Online</a>
      <a href="#kontak">Kontak</a>
    </nav>
  </header>

  <!-- Banner -->
  <div class="banner">
    <div>
      <h2>Nikmati Sajian Autentik<br>Dengan Cita Rasa Asli</h2>
      <a href="#reservasi" class="btn">Reservasi Meja</a>
      <a href="#order" class="btn">Order Online</a>
    </div>
  </div>

  <!-- Highlight Menu -->
  <section class="highlight" id="menu">
    <h2>Menu Favorit Kami</h2>
    <div class="menu-items">
      <div class="menu-card">
        <img src="(https://photos.google.com/album/AF1QipOpYfdXuKLjeG4vpHw92jPs2yoDrcoc8CM1sZZ0/photo/AF1QipP2pCgMsoSpp5K2_CkRwXteF2265jC17KtUuI-Y)/250x150/?steak" alt="Steak" width="100%">
        <h3>Steak Premium</h3>
        <p>Rp 120.000</p>
      </div>
      <div class="menu-card">
        <img src="(https://photos.google.com/album/AF1QipOpYfdXuKLjeG4vpHw92jPs2yoDrcoc8CM1sZZ0/photo/AF1QipOQhgiGZHMn7SULkDuAd8MBcF_Oao9giWXfWpL8)" alt="Pasta" width="100%">
        <h3>Pasta Creamy</h3>
        <p>Rp 75.000</p>
      </div>
      <div class="menu-card">
        <img src="[https://source.unsplash.com](https://photos.google.com/album/AF1QipOpYfdXuKLjeG4vpHw92jPs2yoDrcoc8CM1sZZ0/photo/AF1QipNkDDrZRtcGGyb3jfggyVs1IWZWxoJVMvAm3711)/250x150/?dessert" alt="Dessert" width="100%">
        <h3>Chocolate Lava</h3>
        <p>Rp 45.000</p>
      </div>
    </div>
  </section>

  <!-- Promo -->
  <section class="promo">
    <h2>Promo Hari Ini 🎉</h2>
    <p>Diskon 20% untuk Paket Keluarga (min. 4 orang)!</p>
  </section>

  <!-- Reservasi -->
  <section class="reservasi" id="reservasi">
    <h2>Reservasi Online</h2>
    <form action="mailto:info@restoranlezat.com" method="post" enctype="text/plain">
      <label>Nama Lengkap</label>
      <input type="text" name="nama" required>

      <label>Email</label>
      <input type="email" name="email" required>

      <label>No. Telepon</label>
      <input type="tel" name="telepon" required>

      <label>Tanggal Reservasi</label>
      <input type="date" name="tanggal" required>

      <label>Jam Reservasi</label>
      <input type="time" name="jam" required>

      <label>Jumlah Orang</label>
      <select name="jumlah">
        <option>2 Orang</option>
        <option>4 Orang</option>
        <option>6 Orang</option>
        <option>8 Orang</option>
        <option>10+ Orang</option>
      </select>

      <label>Catatan Tambahan</label>
      <textarea name="catatan" rows="4"></textarea>

      <button type="submit">Kirim Reservasi</button>
    </form>
    <p>Atau hubungi via WhatsApp 👉 <a href="https://wa.me/6285643950602" target="_blank">Chat Admin</a></p>
  </section>

  <!-- Order Online -->
  <section class="order" id="order">
    <h2>Order Online (Takeaway / Delivery)</h2>
    <form onsubmit="kirimWA(); return false;">
      <label>Nama Lengkap</label>
      <input type="text" id="nama" required>

      <label>No. WhatsApp</label>
      <input type="tel" id="wa" required>

      <label>Alamat Pengiriman</label>
      <textarea id="alamat" rows="3" required></textarea>

      <label>Pilih Menu</label>
      <select id="menu">
        <option>Steak Premium - Rp 120.000</option>
        <option>Pasta Creamy - Rp 75.000</option>
        <option>Chocolate Lava - Rp 45.000</option>
      </select>

      <label>Jumlah</label>
      <input type="number" id="jumlah" min="1" value="1" required>

      <label>Catatan</label>
      <textarea id="catatan" rows="3"></textarea>

      <button type="submit">Pesan via WhatsApp</button>
    </form>
  </section>

  <!-- About -->
  <section class="about">
    <h2>Tentang Restoran Lezat</h2>
    <p>Kami menghadirkan pengalaman kuliner dengan cita rasa khas nusantara 
    dan internasional, menggunakan bahan segar pilihan dan pelayanan terbaik.</p>
  </section>

  <!-- Footer -->
  <footer id="kontak">
    <p>📍 Jl. Dalangan-tawangsari,Sukoharjo</p>
    <p>📞 0856-4395-0602 | ✉️ info@restoranlezat.com</p>
    <p>© 2025 Restoran Lezat. All rights reserved.</p>
  </footer>

  <!-- Script WhatsApp -->
  <script>
    function kirimWA() {
      let nama = document.getElementById("nama").value;
      let wa = document.getElementById("wa").value;
      let alamat = document.getElementById("alamat").value;
      let menu = document.getElementById("menu").value;
      let jumlah = document.getElementById("jumlah").value;
      let catatan = document.getElementById("catatan").value;

      let pesan = `Halo Admin, saya ingin order online:%0A
      Nama: ${nama}%0A
      No. WA: ${wa}%0A
      Alamat: ${alamat}%0A
      Menu: ${menu}%0A
      Jumlah: ${jumlah}%0A
      Catatan: ${catatan}`;

      window.open(`https://wa.me/6285643950602?text=${pesan}`, "_blank");
    }
  </script>

</body>
</html>
