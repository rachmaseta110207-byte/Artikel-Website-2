
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portofolio Pribadi</title>

    <!-- AOS CSS -->
    <link href="https://unpkg.com/aos@2.3.4/dist/aos.css" rel="stylesheet">

    <!-- Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', sans-serif; }

        body {
            background: linear-gradient(135deg, #e3f2fd, #f1f8ff);
            color: #333;
            scroll-snap-type: y mandatory;
            overflow-y: scroll;
        }

        body::before {
            content: "";
            position: fixed;
            inset: 0;
            background-image:
                linear-gradient(rgba(0,0,0,0.04) 1px, transparent 1px),
                linear-gradient(90deg, rgba(0,0,0,0.04) 1px, transparent 1px);
            background-size: 35px 35px;
            pointer-events: none;
            z-index: -1;
        }

        header { text-align: center; padding: 40px 20px; color: white; }

        header img {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            border: 4px solid white;
            margin-bottom: 10px;
        }

        nav {
            background: white;
            display: flex;
            justify-content: center;
            padding: 10px;
            gap: 20px;
            position: sticky;
            top: 0;
        }

        nav a { text-decoration: none; color: #333; font-weight: bold; }
        nav a:hover { color: #764ba2; }

        .container { width: 85%; margin: 20px auto; }

        .card {
            background: white;
            margin: 20px 0;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        h2 { margin-bottom: 10px; color: #764ba2; }

        ul { margin-left: 20px; }

        footer { text-align: center; padding: 15px; color: white; }

        /* SOCIAL */
        .social {
            position: fixed;
            right: 15px;
            bottom: 20px;
            display: flex;
            flex-direction: column;
            gap: 12px;
        }

        .social a {
            width: 45px;
            height: 45px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
            color: white;
            font-size: 18px;
            transition: 0.3s;
            box-shadow: 0 4px 10px rgba(0,0,0,0.2);
        }

        /* warna asli + efek */
        .wa { background: #25D366; }
        .ig { background: radial-gradient(circle at 30% 107%, #fdf497 0%, #fd5949 45%, #d6249f 60%, #285AEB 90%); }
        .tt { background: black; }
        .fb { background: #1877F2; }

        /* efek hover glow */
        .social a:hover {
            transform: scale(1.15);
            box-shadow: 0 0 15px rgba(0,0,0,0.4);
        }

    </style>
</head>
<body>

<header data-aos="fade-down">
    <img src="foto profil.jpeg" alt="Foto Profil">
    <h1>Suwono</h1>
    <p>Pekerja | Kreator </p>
</header>

<nav data-aos="fade-up">
    <a href="#data">Data</a>
    <a href="#pendidikan">Pendidikan</a>
    <a href="#hobi">Hobi</a>
    <a href="#moto">Moto</a>
</nav>

<div class="container">

    <div class="card" id="data" data-aos="fade-right">
        <h2>Data Diri</h2>
        <p>Nama: Suwono</p>
        <p>TTL:Malang, 14 April 1993 </p>
        <p>Alamat:Pakis Kembar</p>
    </div>

    <div class="card" id="pendidikan" data-aos="fade-left">
        <h2>Riwayat Pendidikan</h2>
        <ul>
            <li>SD/MI[Hasyim Asy'ary]</li>
            <li>SMP/SMA[SMP nu04pakis] </li>
            <li>SMK/SMA[SMK Ma'arifnu04pakis]</li>
        </ul>
    </div>

    <div class="card" id="hobi" data-aos="zoom-in">
        <h2>Hobi</h2>
        <ul>
            <li>Olahraga</li>
        </ul>
    </div>

    <div class="card" id="moto" data-aos="fade-up">
        <h2>Moto</h2>
        <p>Selalu Tersenyum apapun keadaanmu</p>
    </div>

</div>

<div class="social">
    <a href="https://wa.me/628xxxxxxxxxx?text=Halo%20saya%20tertarik%20dengan%20profil%20anda" class="wa" target="_blank"><i class="fab fa-whatsapp"></i></a>
    <a href="#" class="ig" target="_blank"><i class="fab fa-instagram"></i></a>
    <a href="#" class="tt" target="_blank"><i class="fab fa-tiktok"></i></a>
    <a href="#" class="fb" target="_blank"><i class="fab fa-facebook-f"></i></a>
</div>

<footer data-aos="fade-up">
    <p>&copy; 2026 Portofolio</p>
</footer>

<script src="https://unpkg.com/aos@2.3.4/dist/aos.js"></script>
<script>
    AOS.init({ duration: 1000, once: true });
</script>

</body>
</html>
