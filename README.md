<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Clikanet Telecom - Internet Fibra 1 Giga em Arapiraca</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body { font-family: Arial, sans-serif; background: #f4f4f4; color: #333; line-height: 1.6; }
    a { text-decoration: none; }

    /* Cabeçalho */
    header {
      background: #003366;
      color: white;
      text-align: center;
      padding: 1.5rem;
    }
    .logo { font-size: 2rem; font-weight: bold; }
    .logo span { color: #00ccff; }

    /* Banner */
    .banner {
      background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('https://images.unsplash.com/photo-1519389950477-546f77f2f50a?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80') center/cover;
      color: white;
      text-align: center;
      padding: 100px 20px;
    }
    .banner h1 { font-size: 2.5rem; margin-bottom: 1rem; }
    .btn {
      background: #00ccff;
      color: white;
      padding: 12px 30px;
      border-radius: 30px;
      font-weight: bold;
      display: inline-block;
      margin: 10px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.2);
    }
    .btn:hover { background: #0099cc; }

    /* Planos */
    .planos { padding: 50px 20px; text-align: center; background: white; }
    .planos h2 { margin-bottom: 30px; color: #003366; }
    .plano-card {
      background: #f9f9f9;
      border: 2px solid #ddd;
      border-radius: 15px;
      padding: 20px;
      margin: 15px auto;
      max-width: 300px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    }
    .plano-card.destaque { border-color: #00ccff; background: #e6f7ff; }
    .preco { font-size: 2rem; color: #00ccff; font-weight: bold; }
    .preco small { font-size: 1rem; color: #666; }

    /* Cobertura */
    .cobertura { padding: 50px 20px; background: #f0f8ff; text-align: center; }
    input[type="text"] {
      width: 100%;
      max-width: 300px;
      padding: 12px;
      margin: 10px 0;
      border: 2px solid #ccc;
      border-radius: 10px;
      font-size: 1rem;
    }
    #resultado { margin-top: 15px; font-weight: bold; }

    /* Contato */
    .contato { padding: 50px 20px; text-align: center; background: white; }
    .contato-info { margin: 20px 0; }
    .contato-info i { color: #00ccff; margin-right: 8px; }

    /* Rodapé */
    footer {
      background: #003366;
      color: white;
      text-align: center;
      padding: 20px;
      font-size: 0.9rem;
    }

    /* WhatsApp Flutuante */
    .whatsapp {
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
      box-shadow: 0 5px 15px rgba(0,0,0,0.3);
      z-index: 999;
    }

    /* Mobile */
    @media (max-width: 600px) {
      .banner h1 { font-size: 2rem; }
      .btn { display: block; margin: 10px auto; width: 200px; }
    }
  </style>
</head>
<body>

  <!-- Cabeçalho -->
  <header>
    <div class="logo">Clika<span>net</span> Telecom</div>
  </header>

  <!-- Banner -->
  <section class="banner">
    <h1>Internet Fibra até <span style="color:#00ccff">1 GIGA</span></h1>
    <p>Velocidade real, suporte local e instalação grátis!</p>
    <a href="https://wa.me/5582999582737" class="btn" target="_blank">Falar no WhatsApp</a>
    <a href="#planos" class="btn">Ver Planos</a>
  </section>

  <!-- Planos -->
  <section class="planos" id="planos">
    <h2>Nossos Planos</h2>
    <div class="plano-card">
      <h3>200 Mega</h3>
      <div class="preco">R$79,90<small>/mês</small></div>
      <p>Perfeito para casa</p>
      <a href="https://wa.me/5582999582737" class="btn" target="_blank">Contratar</a>
    </div>
    <div class="plano-card">
      <h3>500 Mega</h3>
      <div class="preco">R$99,90<small>/mês</small></div>
      <p>Streaming e jogos</p>
      <a href="https://wa.me/5582999582737" class="btn" target="_blank">Contratar</a>
    </div>
    <div class="plano-card destaque">
      <h3>1 GIGA</h3>
      <div class="preco">R$149,90<small>/mês</small></div>
      <p>Velocidade máxima</p>
      <a href="https://wa.me/5582999582737" class="btn" target="_blank">Contratar Agora</a>
    </div>
  </section>

  <!-- Verificador de Cobertura -->
  <section class="cobertura">
    <h2>Verifique a Cobertura</h2>
    <input type="text" id="cep" placeholder="Digite seu CEP (ex: 57300000)" maxlength="8"/>
    <button class="btn" onclick="verificar()">Verificar</button>
    <div id="resultado"></div>
  </section>

  <!-- Contato -->
  <section class="contato">
    <h2>Entre em Contato</h2>
    <div class="contato-info">
      <p><i class="fas fa-phone"></i> (82) 99958-2737</p>
      <p><i class="fas fa-map-marker-alt"></i> Rua São Cristóvão, 1024 - Centro, Arapiraca</p>
      <p><i class="fas fa-envelope"></i> contato@clikanet.com.br</p>
    </div>
    <a href="https://wa.me/5582999582737" class="btn" target="_blank">Falar no WhatsApp</a>
  </section>

  <!-- Rodapé -->
  <footer>
    <p>&copy; 2025 Clikanet Telecom. Todos os direitos reservados.</p>
  </footer>

  <!-- WhatsApp Flutuante -->
  <a href="https://wa.me/5582999582737" class="whatsapp" target="_blank">
    <i class="fab fa-whatsapp"></i>
  </a>

  <!-- Ícones (Font Awesome) -->
  <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>

  <!-- Script Simples -->
  <script>
    function verificar() {
      const cep = document.getElementById('cep').value;
      const res = document.getElementById('resultado');
      if (cep.length === 8 && !isNaN(cep)) {
        res.innerHTML = '<span style="color:green">Cobertura DISPONÍVEL no seu CEP!</span>';
      } else {
        res.innerHTML = '<span style="color:red">Digite um CEP válido (8 números).</span>';
      }
    }
  </script>

</body>
</html>
