# Agro-sustentabilidade

"Agro forte, futuro sustentável: equilíbrio entre produção e meio ambiente"

<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Agro Forte | Futuro Sustentável</title>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

  <style>

    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:'Poppins', sans-serif;
    }

    html{
      scroll-behavior:smooth;
    }

    body{
      background:#f4fff4;
      color:#1d2b1f;
      transition:0.4s;
      overflow-x:hidden;
    }

    /* NAVBAR */

    nav{
      position:fixed;
      top:0;
      width:100%;
      display:flex;
      justify-content:space-between;
      align-items:center;
      padding:18px 8%;
      background:rgba(0,0,0,0.4);
      backdrop-filter:blur(10px);
      z-index:999;
    }

    .logo{
      color:white;
      font-size:1.5rem;
      font-weight:700;
    }

    nav ul{
      display:flex;
      gap:25px;
      list-style:none;
    }

    nav a{
      color:white;
      text-decoration:none;
      font-weight:500;
      transition:0.3s;
    }

    nav a:hover{
      color:#8cff98;
    }

    /* HERO */

    .hero{
      height:100vh;

      background:
      linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)),
      url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1600&auto=format&fit=crop');

      background-size:cover;
      background-position:center;

      display:flex;
      align-items:center;
      justify-content:center;
      text-align:center;
      color:white;
      padding:20px;
    }

    .hero-content{
      max-width:850px;
      animation:fade 1.5s ease;
    }

    .hero h1{
      font-size:5rem;
      margin-bottom:20px;
      line-height:1.1;
    }

    .hero span{
      color:#8cff98;
    }

    .hero p{
      font-size:1.3rem;
      margin-bottom:35px;
      line-height:1.8;
    }

    .hero-btn{
      padding:15px 35px;
      background:#4CAF50;
      color:white;
      text-decoration:none;
      border-radius:50px;
      font-weight:600;
      transition:0.3s;
      display:inline-block;
    }

    .hero-btn:hover{
      transform:translateY(-5px);
      background:#2e7d32;
    }

    /* SEÇÕES */

    section{
      padding:100px 10%;
    }

    .titulo{
      text-align:center;
      font-size:3rem;
      margin-bottom:20px;
      color:#2e7d32;
    }

    .subtitulo{
      text-align:center;
      max-width:800px;
      margin:auto;
      margin-bottom:60px;
      color:#555;
      line-height:1.8;
    }

    /* CARDS */

    .cards{
      display:grid;
      grid-template-columns:repeat(auto-fit, minmax(320px,1fr));
      gap:30px;
    }

    .card{
      background:white;
      border-radius:25px;
      overflow:hidden;
      box-shadow:0 10px 25px rgba(0,0,0,0.1);
      transition:0.4s;
      position:relative;
    }

    .card:hover{
      transform:translateY(-12px);
      box-shadow:0 15px 35px rgba(0,0,0,0.2);
    }

    .card img{
      width:100%;
      height:260px;
      object-fit:cover;
    }

    .card-content{
      padding:25px;
    }

    .card h3{
      margin-bottom:15px;
      color:#2e7d32;
      font-size:1.5rem;
    }

    .card p{
      color:#555;
      line-height:1.8;
    }

    /* BANNER */

    .banner{
      padding:140px 10%;

      background:
      linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)),
      url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?q=80&w=1600&auto=format&fit=crop');

      background-size:cover;
      background-position:center;

      text-align:center;
      color:white;
    }

    .banner h2{
      font-size:4rem;
      margin-bottom:20px;
    }

    .banner p{
      max-width:800px;
      margin:auto;
      line-height:1.8;
      font-size:1.2rem;
    }

    /* GRID TEXTO + IMAGEM */

    .conteudo{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:50px;
      align-items:center;
      margin-top:60px;
    }

    .conteudo img{
      width:100%;
      border-radius:25px;
      box-shadow:0 10px 25px rgba(0,0,0,0.2);
    }

    .conteudo-texto h3{
      font-size:2rem;
      margin-bottom:20px;
      color:#2e7d32;
    }

    .conteudo-texto p{
      line-height:1.9;
      margin-bottom:20px;
      color:#444;
    }

    /* GALERIA */

    .galeria{
      display:grid;
      grid-template-columns:repeat(auto-fit, minmax(250px,1fr));
      gap:20px;
    }

    .galeria img{
      width:100%;
      height:280px;
      object-fit:cover;
      border-radius:20px;
      transition:0.4s;
    }

    .galeria img:hover{
      transform:scale(1.05);
    }

    /* FOOTER */

    footer{
      background:#163b18;
      color:white;
      text-align:center;
      padding:40px;
    }

    /* ACESSIBILIDADE */

    .acessibilidade{
      position:fixed;
      right:20px;
      bottom:20px;
      display:flex;
      flex-direction:column;
      gap:12px;
      z-index:1000;
    }

    .acessibilidade button{
      width:55px;
      height:55px;
      border:none;
      border-radius:50%;
      background:#2e7d32;
      color:white;
      font-size:18px;
      cursor:pointer;
      transition:0.3s;
      box-shadow:0 5px 15px rgba(0,0,0,0.3);
    }

    .acessibilidade button:hover{
      transform:scale(1.1);
      background:#1b5e20;
    }

    /* MODO ESCURO */

    .dark-mode{
      background:#121212;
      color:white;
    }

    .dark-mode .card{
      background:#1e1e1e;
    }

    .dark-mode .card p,
    .dark-mode .conteudo-texto p,
    .dark-mode .subtitulo{
      color:#d8d8d8;
    }

    .dark-mode footer{
      background:#000;
    }

    .dark-mode .titulo,
    .dark-mode .conteudo-texto h3{
      color:#8cff98;
    }

    /* ANIMAÇÃO */

    @keyframes fade{

      from{
        opacity:0;
        transform:translateY(40px);
      }

      to{
        opacity:1;
        transform:translateY(0);
      }

    }

    /* RESPONSIVO */

    @media(max-width:900px){

      .hero h1{
        font-size:3rem;
      }

      .conteudo{
        grid-template-columns:1fr;
      }

      nav{
        flex-direction:column;
        gap:15px;
      }

    }

  </style>
</head>

<body>

  <!-- NAV -->

  <nav>

    <div class="logo">🌱 Agro Forte</div>

    <ul>
      <li><a href="#sobre">Sobre</a></li>
      <li><a href="#tecnologia">Tecnologia</a></li>
      <li><a href="#galeria">Galeria</a></li>
    </ul>

  </nav>

  <!-- ACESSIBILIDADE -->

  <div class="acessibilidade">
    <button onclick="aumentarFonte()">A+</button>
    <button onclick="diminuirFonte()">A-</button>
    <button onclick="alternarTema()">🌙</button>
  </div>

  <!-- HERO -->

  <section class="hero">

    <div class="hero-content">

      <h1>
        Agro Forte <br>
        <span>Futuro Sustentável</span>
      </h1>

      <p>
        O equilíbrio entre produção agrícola e preservação ambiental é o caminho
        para garantir alimentos, desenvolvimento econômico e qualidade de vida
        para as futuras gerações.
      </p>

      <a href="#sobre" class="hero-btn">
        Descobrir Mais
      </a>

    </div>

  </section>

  <!-- SOBRE -->

  <section id="sobre">

    <h2 class="titulo">O Agro do Futuro</h2>

    <p class="subtitulo">
      O agronegócio sustentável busca unir tecnologia, inovação e responsabilidade ambiental.
      Hoje, produtores rurais utilizam práticas modernas para aumentar a produtividade sem
      prejudicar a natureza.
    </p>

    <div class="cards">

      <div class="card">

        <img src="https://images.unsplash.com/photo-1464226184884-fa280b87c399?q=80&w=1200&auto=format&fit=crop">

        <div class="card-content">

          <h3>Produção Sustentável</h3>

          <p>
            Métodos agrícolas modernos ajudam a economizar água, preservar o solo
            e reduzir impactos ambientais, garantindo alimentos de qualidade.
          </p>

        </div>

      </div>

      <div class="card">

        <img src="https://images.unsplash.com/photo-1501004318641-b39e6451bec6?q=80&w=1200&auto=format&fit=crop">

        <div class="card-content">

          <h3>Preservação Ambiental</h3>

          <p>
            O cuidado com florestas, rios e biodiversidade é essencial para manter
            o equilíbrio ecológico e proteger os recursos naturais.
          </p>

        </div>

      </div>

      <div class="card">

        <img src="https://images.unsplash.com/photo-1492496913980-501348b61469?q=80&w=1200&auto=format&fit=crop">

        <div class="card-content">

          <h3>Tecnologia no Campo</h3>

          <p>
            Sensores, drones e inteligência artificial tornam o campo mais eficiente,
            produtivo e sustentável.
          </p>

        </div>

      </div>

    </div>

  </section>

  <!-- BANNER -->

  <section class="banner">

    <h2>Produzir Hoje. Preservar Amanhã.</h2>

    <p>
      A sustentabilidade no campo é um compromisso com o futuro do planeta,
      garantindo equilíbrio entre economia, sociedade e meio ambiente.
    </p>

  </section>

  <!-- TECNOLOGIA -->

  <section id="tecnologia">

    <h2 class="titulo">Tecnologia e Sustentabilidade</h2>

    <p class="subtitulo">
      A inovação no campo transforma a agricultura em uma atividade mais inteligente,
      eficiente e sustentável.
    </p>

    <div class="conteudo">

      <img src="https://images.unsplash.com/photo-1502082553048-f009c37129b9?q=80&w=1200&auto=format&fit=crop">

      <div class="conteudo-texto">

        <h3>Inovação no Campo</h3>

        <p>
          A agricultura moderna utiliza recursos tecnológicos para monitorar plantações,
          analisar o clima e reduzir desperdícios. Isso permite uma produção mais eficiente
          e com menor impacto ambiental.
        </p>

        <p>
          Sistemas inteligentes ajudam produtores a economizar água, energia e fertilizantes,
          tornando o agronegócio mais sustentável e preparado para os desafios do futuro.
        </p>

      </div>

    </div>

    <div class="conteudo">

      <div class="conteudo-texto">

        <h3>Energia Renovável</h3>

        <p>
          Muitas propriedades rurais já utilizam energia solar e outras fontes renováveis
          para reduzir custos e diminuir a emissão de poluentes.
        </p>

        <p>
          Essas práticas contribuem para um planeta mais limpo e fortalecem o compromisso
          do agro com o desenvolvimento sustentável.
        </p>

      </div>

      <img src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?q=80&w=1200&auto=format&fit=crop">

    </div>

  </section>

  <!-- GALERIA -->

  <section id="galeria">

    <h2 class="titulo">Galeria do Agro</h2>

    <p class="subtitulo">
      Imagens que representam a força do agronegócio aliado à preservação da natureza.
    </p>

    <div class="galeria">

      <img src="https://images.unsplash.com/photo-1500382017468-9049fed747ef?q=80&w=1200&auto=format&fit=crop">

      <img src="https://images.unsplash.com/photo-1499529112087-3cb3b73cec95?q=80&w=1200&auto=format&fit=crop">

      <img src="https://images.unsplash.com/photo-1501004318641-b39e6451bec6?q=80&w=1200&auto=format&fit=crop">

      <img src="https://images.unsplash.com/photo-1464226184884-fa280b87c399?q=80&w=1200&auto=format&fit=crop">

      <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?q=80&w=1200&auto=format&fit=crop">

      <img src="https://images.unsplash.com/photo-1502082553048-f009c37129b9?q=80&w=1200&auto=format&fit=crop">

    </div>

  </section>

  <!-- FOOTER -->

  <footer>

    <h3>🌱 Agro Forte</h3>

    <p>
      Futuro Sustentável: equilíbrio entre produção e meio ambiente.
    </p>

  </footer>

  <!-- SCRIPT -->

  <script>

    let tamanhoFonte = 100;

    function aumentarFonte(){

      tamanhoFonte += 10;
      document.body.style.fontSize = tamanhoFonte + "%";

    }

    function diminuirFonte(){

      tamanhoFonte -= 10;

      if(tamanhoFonte < 70){
        tamanhoFonte = 70;
      }

      document.body.style.fontSize = tamanhoFonte + "%";

    }

    function alternarTema(){

      document.body.classList.toggle("dark-mode");

    }

  </script>

</body>
</html>
