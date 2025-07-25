# Simple-Website-Jualan

pertama buat folder di laptop atau pc contoh: landing-page

buka vscode upload folder

buat 3 file berikut didalam folder:
index.html
style.css
assets/ (opsional: isi gambar/logo/icon)

masukan code dibawah ini kedalam file index.html

<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Landing Page Angkringan</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Angkringan Makbik</h1>
    <nav>
      <a href="#about">Tentang</a>
      <a href="#menu">Menu</a>
      <a href="#kontak">Kontak</a>
    </nav>
  </header>

  <section id="hero">
    <h2>Selamat Datang di Angkringan Makbik</h2>
    <p>Rasakan kenikmatan nongkrong dengan view kuburan.</p>
  </section>

  <section id="about">
    <h3>Tentang Kami</h3>
    <p>Angkringan kami berdiri sejak penjajahan belanda.</p>
  </section>

  <section id="menu">
    <h3>Menu Unggulan</h3>
    <ul>
      <li>Nasi kucing</li>
      <li>Sate usus</li>
      <li>Gorengan gacor</li>
      <li>Susu jahe</li>
    </ul>
  </section>

  <section id="kontak">
    <h3>Hubungi Kami</h3>
    <form action="https://formspree.io/f/mgvzkkqz" method="POST">
  <input type="text" name="nama" placeholder="Nama" required>
  <input type="email" name="email" placeholder="Email" required>
  <textarea name="pesan" placeholder="Pesan" required></textarea>
  <button type="submit">Kirim</button>
</form>

  </section>

  <footer>
    <p>&copy; 2025 Angkrian Makbik. All rights reserved.</p>
  </footer>
  <a href="https://wa.me/6283842184068?text=Halo%20saya%20tertarik%20dengan%20kopi%20Anda" 
   class="whatsapp-float" 
   target="_blank" 
   title="Chat via WhatsApp">
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" alt="WhatsApp" />
</a>
</body>
</html>

masukan code dibawah ini kedalam file style.css

body {
  font-family: sans-serif;
  margin: 0;
  padding: 0;
  background: #f8f8f8;
  color: rgb(0, 0, 0);
}

header {
  background: #3e2723;
  color: white;
  padding: 20px;
  text-align: center;
}

nav a {
  color: white;
  margin: 0 10px;
  text-decoration: none;
}

#hero {
  padding: 50px;
  background: url('https://source.unsplash.com/800x400/?coffee') no-repeat center;
  background-size: cover;
  color: rgb(76, 69, 69);
  text-align: center;
}

section {
  padding: 40px;
  background: white;
  margin: 20px;
  border-radius: 8px;
}

form input, form textarea {
  width: 100%;
  margin: 10px 0;
  padding: 10px;
}

button {
  background: #795548;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 6px;
  cursor: pointer;
}

footer {
  background: #3e2723;
  color: white;
  text-align: center;
  padding: 10px;
}

.whatsapp-float {
  position: fixed;
  bottom: 20px;
  right: 20px;
  width: 60px;
  height: 60px;
  z-index: 100;
}

.whatsapp-float img {
  width: 100%;
  height: 100%;
  object-fit: contain;
  border-radius: 50%;
  box-shadow: 0 4px 10px rgba(0,0,0,0.3);
  transition: transform 0.2s ease;
}

.whatsapp-float img:hover {
  transform: scale(1.1);
}

