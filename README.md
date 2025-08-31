[index.html](https://github.com/user-attachments/files/22062548/index.html)
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Login</title>
  <link href="https://fonts.googleapis.com/css2?family=Droid+Sans:wght@700&display=swap" rel="stylesheet">
  <style>
    * { box-sizing: border-box; }
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      height: 100vh;
      background-color: #f0f0f0;
      overflow: auto;
    }

    .header {
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 0 20px;
      background-color: #fff;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      height: 120px;
      z-index: 1000;
    }
    .logo { position: absolute; left: 20px; }
    .logo img { max-height: 120px; width: auto; object-fit: contain; }
    .header-title {
      font-family: 'Droid Sans', sans-serif;
      font-size: 60px;
      font-weight: 700;
      color: #333;
      position: absolute;
      left: 50%;
      transform: translateX(-50%);
      white-space: nowrap;
      pointer-events: none;
    }

    .login-box {
      position: fixed;
      right: 20px;
      top: 20px;
      display: flex;
      align-items: center;
      gap: 8px;
      z-index: 1100;
    }
    .login-box input { padding: 6px 8px; font-size: 14px; border: 1px solid #ccc; border-radius: 4px; }
    .login-box button { padding: 6px 12px; font-size: 14px; background-color: red; color: white; border: none; border-radius: 4px; cursor: pointer; transition:0.2s; }
    .login-box button:hover { background-color: darkred; }

    .sidebar-left, .sidebar-right {
      width: 200px;
      background-color: #fff;
      height: calc(100vh - 120px);
      padding: 20px;
      position: fixed;
      top: 120px;
      overflow-y: auto;
    }
    .sidebar-left { left: 0; box-shadow: 2px 0 5px rgba(0,0,0,0.1); }
    .sidebar-right { right: 0; box-shadow: -2px 0 5px rgba(0,0,0,0.1); }

    .center-content {
      position: absolute;
      top: 120px;
      left: 200px;
      right: 200px;
      bottom: 0;
      padding: 20px;
      overflow: auto;
      min-width: 600px;
      text-align: center;
      background-color: #f0f0f0;
    }

    .news-item h2 { font-size: 28px; color: #222; margin: 10px 0 10px; }
    .news-title { font-size: 22px; font-weight: bold; line-height: 1.4; margin-bottom: 15px; color:#555; }
    .news-item img { max-width: 320px; height: auto; margin-top: 10px; border-radius: 6px; box-shadow: 0 2px 5px rgba(0,0,0,0.1); }
    .news-item + .news-item { margin-top: 40px; }
    .isi-tragedi-1998 { text-align: left; margin-top: 20px; color:#555; line-height:1.5; }

    /* BARU: Styling foto sidebar kiri */
    .sidebar-photos {
      display: flex;
      flex-direction: column;
      justify-content: space-between; /* jarak merata */
      height: calc(100% - 60px); /* sisakan padding atas/bawah */
      padding-top: 20px;
      padding-bottom: 20px;
    }
    .sidebar-photos img {
      width: 100%;
      height: auto;
      border-radius: 6px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
  </style>
</head>
<body>
  <!-- HEADER -->
  <div class="header">
    <div class="logo">
      <img src="logo1.png" alt="Logo Manusia Biasa">
    </div>
    <div class="header-title">MANUSIA BIASA</div>
  </div>

  <!-- LOGIN -->
  <div class="login-box">
    <input type="text" placeholder="Username" required>
    <input type="password" placeholder="Password" required>
    <button type="submit">Login</button>
  </div>

  <!-- SIDEBAR KIRI -->
  <div class="sidebar-left">
    <p></p>

    <!-- BARU: Foto di sidebar kiri -->
    <div class="sidebar-photos">
      <img src="kiri1.png" alt="Foto 1">
      <img src="kiri2.png" alt="Foto 2">
      <img src="kiri3.png" alt="Foto 3">
    </div>
  </div>

  <!-- SIDEBAR KANAN -->
  <div class="sidebar-right">
    <p>Konten Sidebar Kanan</p>
    <p>Item A</p>
    <p>Item B</p>
  </div>

  <!-- KONTEN TENGAH SCROLLABLE -->
  <div class="center-content">
    <div class="news-item">
      <h2>Tragedi Mei 1998</h2>
      <p class="news-title">
        Kerusuhan Mei 1998 menjadi salah satu peristiwa paling kelam dalam sejarah Indonesia, yang hingga kini masih sering dibicarakan dan diteliti.
      </p>
      <img src="tragedi1998.png" alt="Tragedi 1998">
      <!-- TEKS TAMBAHAN -->
      <div class="isi-tragedi-1998">
        <p>Kerusuhan Mei 1998, juga dikenal sebagai Tragedi 1998 atau Peristiwa 98, adalah peristiwa kekerasan massal dan kerusuhan sipil di Indonesia pada bulan Mei 1998, yang sebagian besar menargetkan komunitas Tionghoa di negara tersebut. Peristiwa ini terutama terjadi di kota Medan, Jakarta, dan Surakarta, dengan insiden-insiden lebih kecil terjadi di wilayah lain Indonesia.</p>
        <p>Di bawah pemerintahan Soeharto yang didukung Barat, terdapat diskriminasi yang meluas dan sistemik terhadap etnis Tionghoa di Indonesia. Kerusuhan tersebut dipicu oleh korupsi, permasalahan ekonomi, termasuk kekurangan pangan dan pengangguran massal. Kerusuhan ini akhirnya berujung pada pengunduran diri Presiden Soeharto dan jatuhnya pemerintahan Orde Baru, yang telah berkuasa selama 32 tahun dan didukung oleh kekuatan Barat seperti Amerika Serikat. Target utama dari kerusuhan tersebut adalah etnis Tionghoa Indonesia, tetapi sebagian besar korban jiwa disebabkan oleh kebakaran besar dan terjadi di antara para penjarah.</p>
        <p>Diperkirakan lebih dari seribu orang tewas dalam kerusuhan tersebut. Sedikitnya 168 kasus pemerkosaan dilaporkan, dan kerusakan material senilai lebih dari Rp3,1 triliun (US$260 juta). Hingga tahun 2010, proses hukum atas kerusuhan tersebut terhambat dan tidak diselesaikan.</p>
        <p>Bentrokan antara mahasiswa Universitas Trisakti dan aparat kepolisian pada Mei 1998. Pada kerusuhan ini banyak toko dan perusahaan dihancurkan oleh amukan massa—terutama milik warga Indonesia keturunan Tionghoa. Konsentrasi kerusuhan terbesar terjadi di Jakarta, Medan, dan Surakarta. Dalam kerusuhan tersebut, banyak warga Indonesia keturunan Tionghoa yang meninggalkan Indonesia. Tak hanya itu, seorang aktivis relawan kemanusiaan yang bergerak di bawah Romo Sandyawan, bernama Ita Martadinata Haryono, yang masih seorang siswi SMU berusia 18 tahun, juga diperkosa, disiksa, dan dibunuh karena aktivitasnya. Ini menjadi indikasi bahwa kasus pemerkosaan dalam kerusuhan ini digerakkan secara sistematis, tak hanya sporadis.</p>
        <p>Amukan massa ini membuat para pemilik toko di kedua kota tersebut ketakutan dan menulisi muka toko mereka dengan tulisan "Milik pribumi" atau "Pro-reformasi" karena penyerang hanya fokus ke orang-orang Tionghoa. Beberapa dari mereka tidak ketahuan, tetapi ada juga yang ketahuan bukan milik pribumi. Sebagian masyarakat mengasosiasikan peristiwa ini dengan peristiwa Kristallnacht di Jerman pada tanggal 9 November 1938.</p>
        <p>Sampai bertahun-tahun berikutnya Pemerintah Indonesia belum mengambil tindakan apapun terhadap nama-nama yang dianggap kunci dari peristiwa kerusuhan Mei 1998. Pemerintah mengeluarkan pernyataan yang menyebutkan bahwa bukti-bukti konkret tidak dapat ditemukan atas kasus-kasus pemerkosaan tersebut, tetapi pernyataan ini dibantah oleh banyak pihak.</p>
        <p>Sebab dan alasan kerusuhan ini masih banyak diliputi ketidakjelasan dan kontroversi sampai hari ini. Namun umumnya masyarakat Indonesia secara keseluruhan setuju bahwa peristiwa ini merupakan sebuah lembaran hitam sejarah Indonesia, sementara beberapa pihak, terutama pihak Tionghoa, berpendapat ini merupakan tindakan pembasmian (genosida) terhadap orang Tionghoa.</p>
        <p>Source by : Wikipedia</p>
      </div>
    </div>
  </div>
</body>
</html>
