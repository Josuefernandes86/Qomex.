<!DOCTYPE html><html lang="pt">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Qomex | Site Profissional</title>
  <meta name="description" content="Site profissional completo com HTML, CSS e JavaScript." />  <!-- ===== ESTILO ===== -->  <style>
    :root{
      --bg:#0b0b0b;
      --card:#151515;
      --primary:#00e0ff;
      --text:#ffffff;
      --muted:#bdbdbd;
    }
    *{ box-sizing:border-box; margin:0; padding:0; }
    body{
      font-family: Arial, Helvetica, sans-serif;
      background:var(--bg);
      color:var(--text);
      line-height:1.6;
    }
    header{
      padding:20px;
      display:flex;
      justify-content:space-between;
      align-items:center;
      border-bottom:1px solid #222;
    }
    header h1{ color:var(--primary); }
    nav a{
      color:var(--text);
      margin-left:15px;
      text-decoration:none;
      font-weight:bold;
    }
    nav a:hover{ color:var(--primary); }

    .hero{
      padding:80px 20px;
      text-align:center;
      background:linear-gradient(180deg,#000,#0f0f0f);
    }
    .hero h2{ font-size:2.2rem; margin-bottom:15px; }
    .hero p{ color:var(--muted); max-width:600px; margin:0 auto 25px; }
    .btn{
      background:var(--primary);
      color:#000;
      padding:12px 25px;
      border:none;
      border-radius:8px;
      font-weight:bold;
      cursor:pointer;
    }
    .btn:hover{ opacity:.85; }

    section{ padding:60px 20px; max-width:1100px; margin:auto; }
    .cards{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
      gap:20px;
    }
    .card{
      background:var(--card);
      padding:25px;
      border-radius:12px;
      box-shadow:0 10px 25px rgba(0,0,0,.4);
    }
    .card h3{ color:var(--primary); margin-bottom:10px; }

    form{
      max-width:400px;
      margin:auto;
      display:flex;
      flex-direction:column;
      gap:15px;
    }
    input{
      padding:12px;
      border-radius:8px;
      border:none;
      outline:none;
    }

    footer{
      text-align:center;
      padding:30px;
      border-top:1px solid #222;
      color:var(--muted);
    }

    /* Responsivo */
    @media(max-width:600px){
      .hero h2{ font-size:1.7rem; }
    }
  </style></head>
<body>  <!-- ===== CABEÇALHO ===== -->  <header>
    <h1>Qomex</h1>
    <nav>
      <a href="#">Início</a>
      <a href="#servicos">Serviços</a>
      <a href="#contato">Contato</a>
    </nav>
  </header>  <!-- ===== HERO ===== -->  <div class="hero">
    <h2>A tecnologia que impulsiona o teu futuro</h2>
    <p>Criamos sites, sistemas e soluções digitais modernas para empresas e startups.</p>
    <button class="btn" onclick="alert('Obrigado pelo interesse!')">Quero saber mais</button>
  </div>  <!-- ===== SERVIÇOS ===== -->  <section id="servicos">
    <h2 style="text-align:center;margin-bottom:30px;">O que fazemos</h2>
    <div class="cards">
      <div class="card">
        <h3>Websites</h3>
        <p>Sites rápidos, modernos e responsivos.</p>
      </div>
      <div class="card">
        <h3>Apps</h3>
        <p>Aplicações web e mobile para o teu negócio.</p>
      </div>
      <div class="card">
        <h3>Sistemas</h3>
        <p>Painéis, logins e soluções personalizadas.</p>
      </div>
    </div>
  </section>  <!-- ===== CONTATO ===== -->  <section id="contato">
    <h2 style="text-align:center;margin-bottom:20px;">Contato</h2>
    <form onsubmit="enviar(event)">
      <input type="text" placeholder="Nome Completo" required />
      <input type="email" placeholder="Email" required />
      <input type="text" placeholder="Mensagem" required />
      <button class="btn" type="submit">Enviar</button
    </form>
  </section>  <!-- ===== RODAPÉ ===== -->  <footer>
    © 2026 Qomex. Todos os direitos reservados.
  </footer>  <!-- ===== JAVASCRIPT ===== -->  <script>
    function enviar(e){
      e.preventDefault();
      alert('Mensagem enviada com sucesso!');
    }
  </script></body>
</html>
