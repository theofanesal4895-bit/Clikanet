<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <meta name="description" content="Clikanet Telecom - Internet Fibra Óptica até 1 Giga em Arapiraca, AL. Planos com instalação grátis e suporte local."/>
  <title>Clikanet Telecom | Internet Fibra 1 Giga em Arapiraca</title>

  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet"/>
  <!-- Font Awesome -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"/>
  <!-- AOS Animation -->
  <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet"/>

  <style>
    :root {
      --primary: #00d4ff;
      --secondary: #1a1a1a;
      --accent: #ff6b00;
      --light: #f8f9fa;
      --dark: #212529;
    }
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body { font-family: 'Poppins', sans-serif; background: var(--light); color: var(--dark); line-height: 1.6; }
    a { text-decoration: none; color: inherit; }

    /* Header */
    header {
      background: var(--secondary);
      color: white;
      position: fixed;
      width: 100%;
      top: 0;
      z-index: 1000;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }
    nav { display: flex; justify-content: space-between; align-items: center; padding: 1rem 5%; }
    .logo { font-size: 1.8rem; font-weight: 700; }
    .logo span { color: var(--primary); }
    .nav-links { display: flex; gap: 2rem; }
    .nav-links a { font-weight: 500; transition: 0.3s; }
    .nav-links a:hover { color: var(--primary); }
    .mobile-menu { display: none; font-size: 1.5rem; cursor: pointer; }

    /* Hero */
    .hero {
      background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('https://images.unsplash.com/photo-1558494949-ef010cbdcc31?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80') center/cover;
      color: white;
      text-align: center;
      padding: 180px 5% 100px;
    }
    .hero h1 { font-size: 3.5rem; margin-bottom: 1rem; }
    .hero p { font-size: 1.3rem; max-width: 700px; margin: 0 auto 2rem; }
    .btn {
      background: var(--primary);
      color: white;
      padding: 1rem 2rem;
      border-radius: 50px;
      font-weight: 600;
      display: inline-block;
      margin: 0.5rem;
      transition: 0.3s;
      box-shadow: 0 5px 15px rgba(0,212,255,0.3);
    }
    .btn:hover { transform: translateY(-3px); box-shadow: 0 8px 20px rgba(0,212,255,0.4); }
    .btn-secondary { background: var(--accent); box-shadow: 0 5px 15px rgba(255,107,0,0.3); }

    /* Plans */
    .plans { padding: 80px 5%; background: white; text-align: center; }
    .section-title { font-size: 2.5rem; margin-bottom: 3rem; color: var(--secondary); }
    .plan-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 2rem; }
    .plan-card {
      background: white;
      border-radius: 15px;
      padding: 2rem;
      box-shadow: 0 10px 30px rgba(0,0,0,0.1);
      transition: 0.3s;
      border: 3px solid transparent;
    }
    .plan-card:hover { transform: translateY(-10px); border-color: var(--primary); }
    .plan-card.featured { border-color: var(--primary); background: linear-gradient(135deg, #e3faff, #f0faff); }
    .plan-card h3 { font-size: 1.8rem; margin: 1rem 0; }
    .price { font-size: 2.5rem; font-weight: 700; color: var(--primary); }
    .price small { font-size: 1rem; color: #666; }
    .features { list-style: none; margin: 1.5rem 0; text-align: left; }
    .features li { padding: 0.5rem 0; }
    .features i { color: var(--primary); margin-right: 0.5rem; }

    /* Coverage Checker */
    .coverage { padding: 80px 5%; background: #f1f1f1; text-align: center; }
    .form-group { max-width: 500px; margin: 0 auto 2rem; }
    input[type="text"] {
      width: 100%;
      padding: 1rem;
      border: 2px solid #ddd;
      border-radius: 10px;
      font-size: 1.1rem;
    }
    #coverage-result { margin-top: 1.5rem; font-weight: 600; }

    /* TV Section */
    .tv { padding: 80px 5%; background: var(--secondary); color: white; text-align: center; }
    .streaming-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 2rem; margin-top: 2rem; }
    .stream-card {
      background: rgba(255,255,255,0.1);
      padding: 1.5rem;
      border-radius: 15px;
      backdrop-filter: blur(10px);
    }
    .stream-card.coming { opacity: 0.6; }
    .stream-card h4 { margin: 1rem 0; }

    /* Gallery */
    .gallery { padding: 80px 5%; background: white; }
    .gallery-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 1rem; }
    .gallery-img { width: 100%; height: 200px; object-fit: cover; border-radius: 10px; transition: 0.3s; }
    .gallery-img:hover { transform: scale(1.05); }

    /* Testimonials */
    .testimonials { padding: 80px 5%; background: #f8f9fa; text-align: center; }
    .testimonial { max-width: 600px; margin: 2rem auto; font-style: italic; }
    .stars { color: #ffd700; margin: 1rem 0; }

    /* Contact */
    .contact { padding: 80px 5%; background: white; }
    .contact-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 3rem; }
    .map { height: 300px; border-radius: 15px; overflow: hidden; }
    .contact-info h3 { margin-bottom: 1rem; color: var(--primary); }

    /* Footer */
    footer { background: var(--secondary); color: white; text-align: center; padding: 3rem 5% 1.5rem; }
    .social-links { margin: 1.5rem 0; }
    .social-links a { font-size: 1.5rem; margin: 0 1rem; color: white; transition: 0.3s; }
    .social-links a:hover { color: var(--primary); }

    /* WhatsApp Float */
    .whatsapp-float {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #25d366;
      color: white;
      width: 60px;
      height: 60px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 2rem;
      box-shadow: 0 5px 15px rgba(37,211,102,0.4);
      z-index: 999;
      animation: pulse 2s infinite;
    }
    @keyframes pulse { 0% { box-shadow: 0 0 0 0 rgba(37,211,102,0.7); } 70% { box-shadow: 0 0 0 15px rgba(37,211,102,0); } 100% { box-shadow: 0 0 0 0 rgba(37,211,102,0); } }

    /* Counter */
    .counter { font-size: 3rem; font-weight: 700; color: var(--primary); }

    /* Mobile */
    @media (max-width: 768px) {
      .nav-links { display: none; position: absolute; top: 100%; left: 0; width: 100%; background: var(--secondary); flex-direction: column; padding: 1rem 0; }
      .nav-links.active { display: flex; }
      .mobile-menu { display: block; }
      .hero h1 { font-size: 2.5rem; }
      .hero { padding: 150px 5% 80px; }
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <nav>
      <div class="logo">Clika<span>net</span></div>
      <div class="nav-links" id="navLinks">
        <a href="#home">Início</a>
        <a href="#plans">Planos</a>
        <a href="#coverage">Cobertura</a>
        <a href="#tv">TV</a>
        <a href="#contact">Contato</a>
      </div>
      <div class="mobile-menu" onclick="toggleMenu()">☰</div>
    </nav>
  </header>

  <!-- Hero -->
  <section class="hero" id="home" data-aos="fade-up">
    <h1>Internet Fibra até <span style="color:var(--primary)">1 GIGA</span> em Arapiraca</h1>
    <p>Velocidade real, suporte local e instalação grátis. A internet que você merece!</p>
    <a href="#plans" class="btn">Ver Planos</a>
    <a href="https://wa.me/5582999582737" class="btn btn-secondary" target="_blank">Falar no WhatsApp</a>
  </section>

  <!-- Plans -->
  <section class="plans" id="plans">
    <h2 class="section-title" data-aos="fade-up">Nossos Planos</h2>
    <div class="plan-grid">
      <div class="plan-card" data-aos="fade-up" data-aos-delay="100">
        <h3>200 Mega</h3>
        <div class="price">R$79,90<small>/mês</small></div>
        <ul class="features">
          <li><i class="fas fa-check"></i> Fibra Óptica 100%</li>
          <li><i class="fas fa-check"></i> Sem franquia</li>
          <li><i class="fas fa-check"></i> Wi-Fi incluso</li>
        </ul>
        <a href="https://wa.me/5582999582737" class="btn" target="_blank">Contratar</a>
      </div>
      <div class="plan-card" data-aos="fade-up" data-aos-delay="200">
        <h3>500 Mega</h3>
        <div class="price">R$99,90<small>/mês</small></div>
        <ul class="features">
          <li><i class="fas fa-check"></i> Ideal para streaming</li>
          <li><i class="fas fa-check"></i> Suporte 24h</li>
          <li><i class="fas fa-check"></i> Instalação grátis</li>
        </ul>
        <a href="https://wa.me/5582999582737" class="btn" target="_blank">Contratar</a>
      </div>
      <div class="plan-card featured" data-aos="fade-up" data-aos-delay="300">
        <h3>1 GIGA</h3>
        <div class="price">R$149,90<small>/mês</small></div>
        <ul class="features">
          <li><i class="fas fa-check"></i> Velocidade máxima</li>
          <li><i class="fas fa-check"></i> Gamer/Streamer</li>
          <li><i class=" Whatsapp Float -->
  <a href="https://wa.me/5582999582737" class="whatsapp-float" target="_blank">
    <i class="fab fa-whatsapp"></i>
  </a>

  <!-- Scripts -->
  <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
  <script>
    AOS.init({ duration: 1000 });

    function toggleMenu() {
      document.getElementById("navLinks").classList.toggle("active");
    }

    // Counter Animation
    const counters = document.querySelectorAll('.counter');
    const speed = 200;

    const animateCounter = (counter) => {
      const target = +counter.getAttribute('data-target');
      const count = +counter.innerText;
      const increment = target / speed;

      if (count < target) {
        counter.innerText = Math.ceil(count + increment);
        setTimeout(() => animateCounter(counter), 1);
      } else {
        counter.innerText = target + '+';
      }
    };

    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          animateCounter(entry.target);
          observer.unobserve(entry.target);
        }
      });
    });

    document.querySelectorAll('.counter').forEach(counter => {
      counter.setAttribute('data-target', counter.innerText.replace('+', ''));
      counter.innerText = '0';
      observer.observe(counter);
    });

    // Coverage Checker (Simulação)
    document.getElementById('checkCoverage')?.addEventListener('click', function() {
      const cep = document.getElementById('cep').value;
      const result = document.getElementById('coverage-result');
      if (cep.length === 8) {
        setTimeout(() => {
          result.innerHTML = `<span style="color:green"><i class="fas fa-check-circle"></i> Cobertura DISPONÍVEL no seu CEP!</span>`;
        }, 1000);
      } else {
        result.innerHTML = `<span style="color:red"><i class="fas fa-times-circle"></i> Digite um CEP válido.</span>`;
      }
    });
  </script>

  <!-- Formspree (Contato) -->
  <script>
    window.addEventListener("DOMContentLoaded", function () {
      var form = document.getElementById("contact-form");
      if (form) {
        form.addEventListener("submit", function () {
          form.innerHTML = "<p style='text-align:center; color:green;'><i class='fas fa-check'></i> Mensagem enviada com sucesso!</p>";
        });
      }
    });
  </script>

</body>
</html>
