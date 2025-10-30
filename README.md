<!doctype html>
<html lang="km">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>គេហទំព័រគំរូ​របស់​អ្នក</title>
  <style>
    :root{
      --accent:#0b78d1;
      --bg:#f7f9fc;
      --card:#ffffff;
      --text:#222;
      font-family: "Segoe UI", Roboto, "Noto Sans Khmer", sans-serif;
    }
    body{margin:0;background:var(--bg);color:var(--text);line-height:1.5}
    header{background:linear-gradient(90deg,var(--accent),#3aa0ff);color:#fff;padding:28px 16px}
    .container{max-width:960px;margin:0 auto;padding:24px}
    nav{display:flex;justify-content:space-between;align-items:center}
    nav a{color:#fff;text-decoration:none;margin-left:12px;font-weight:600}
    .hero{padding:48px 0;text-align:center}
    h1{margin:0 0 12px;font-size:32px}
    p.lead{margin:0 auto;max-width:720px;opacity:.95}
    .grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:16px;margin-top:24px}
    .card{background:var(--card);padding:18px;border-radius:8px;box-shadow:0 6px 18px rgba(20,30,50,.06)}
    .btn{display:inline-block;padding:10px 16px;border-radius:6px;background:var(--accent);color:#fff;text-decoration:none;font-weight:700}
    footer{padding:20px 0;text-align:center;color:#666}
    /* Contact form */
    form input, form textarea{width:100%;padding:10px;margin:8px 0;border:1px solid #ddd;border-radius:6px;font-size:14px}
    @media(min-width:900px){h1{font-size:40px}}
  </style>
</head>
<body>
  <header>
    <div class="container">
      <nav>
        <div style="font-weight:800">ឈ្មោះ​ក្រុមហ៊ុន/របស់អ្នក</div>
        <div>
          <a href="#about">អំពី</a>
          <a href="#services">សេវាកម្ម</a>
          <a href="#contact">ទាក់ទង</a>
        </div>
      </nav>
      <div class="hero">
        <h1>សួស្ដី! ជំរាបសួរ — សូមស្វាគមន៍</h1>
        <p class="lead">នេះគឺគេហទំព័រ​ពណ៌សាមញ្ញ ដែលអាចផ្លាស់ប្តូរប្រកាស/រូបភាព/ពណ៌បានងាយ។</p>
        <p style="margin-top:18px"><a class="btn" href="#contact">ទាក់ទងមកពួកយើង</a></p>
      </div>
    </div>
  </header>

  <main class="container" style="margin-top:18px">
    <section id="about" class="card">
      <h2>អំពីយើង</h2>
      <p>សេចក្ដីពិពណ៌នា​សង្ខេប​អំពីអ្នក ឬក្រុមហ៊ុន — ដាក់អត្ថបទនេះជំនួសបាន។</p>
    </section>

    <section id="services" style="margin-top:16px">
      <div class="grid">
        <div class="card">
          <h3>សេវា A</h3>
          <p>ពណ៌នា សេវាកម្ម A — បង្ហាញអត្ថប្រយោជន៍ខាងក្រោម។</p>
        </div>
        <div class="card">
          <h3>សេវា B</h3>
          <p>ពណ៌នា​សេវាកម្ម B — ពិពណ៌នាខ្លីៗ។</p>
        </div>
        <div class="card">
          <h3>សេវា C</h3>
          <p>ពណ៌នា​សេវាកម្ម C — អ្នកអាចបន្ថែមរូបភាព។</p>
        </div>
      </div>
    </section>

    <section id="contact" class="card" style="margin-top:16px">
      <h2>ទាក់ទងមកយើង</h2>
      <p>បំពេញទម្រង់ខាងក្រោម ឬអ៊ីមែលទៅ <strong>you@example.com</strong></p>

      <!-- Example using mailto (simple) -->
      <form action="mailto:you@example.com" method="post" enctype="text/plain">
        <input type="text" name="name" placeholder="ឈ្មោះ" required>
        <input type="email" name="email" placeholder="អ៊ីមែល" required>
        <textarea name="message" rows="5" placeholder="សាររបស់អ្នក"></textarea>
        <div style="display:flex;gap:8px">
          <button class="btn" type="submit">ផ្ញើ</button>
          <button type="reset" style="padding:10px;border-radius:6px;border:1px solid #ddd;background:#fff">កែសម្រួលលុប</button>
        </div>
      </form>

      <p style="margin-top:12px;font-size:13px;color:#666">ចំណាំ៖ mailto នឹងបើកកម្មវិធីអ៊ីមែលរបស់អ្នក។ ប្រសិនបើចង់ទទួលសារផ្ទាល់លើវែបសាយ (without mail client) — អ្នកអាចប្រើសេវាជំនួយដូចជា Formspree ឬ Getform ដើម្បីទទួល POST ទម្រង់។</p>
    </section>
  </main>

  <footer>
    <div class="container">
      © <span id="year"></span> ឈ្មោះ​របស់អ្នក — ទូរស័ព្ទ: +855 12 345 678
    </div>
  </footer>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
