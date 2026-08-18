<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Velozes e Furiosos - A Saga</title>
  <style>
    :root {
      --bg-color: #121212;
      --card-bg: #1e1e1e;
      --accent-color: #e50914;
      --text-color: #ffffff;
      --text-secondary: #aaaaaa;
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: var(--bg-color);
      color: var(--text-color);
      margin: 0;
      padding: 20px;
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    header {
      text-align: center;
      margin-bottom: 30px;
    }

    h1 {
      color: var(--accent-color);
      text-transform: uppercase;
      letter-spacing: 2px;
      margin-bottom: 5px;
    }

    .tabs-container {
      width: 100%;
      max-width: 900px;
    }

    .tabs-header {
      display: flex;
      flex-wrap: wrap;
      gap: 5px;
      border-bottom: 2px solid #333;
      padding-bottom: 10px;
      justify-content: center;
    }

    .tab-btn {
      background-color: var(--card-bg);
      color: var(--text-color);
      border: 1px solid #333;
      padding: 10px 15px;
      cursor: pointer;
      border-radius: 5px;
      font-weight: bold;
      transition: background 0.3s, color 0.3s;
    }

    .tab-btn:hover {
      background-color: #333;
    }

    .tab-btn.active {
      background-color: var(--accent-color);
      border-color: var(--accent-color);
    }

    .tab-content {
      display: none;
      background-color: var(--card-bg);
      padding: 25px;
      border-radius: 0 0 8px 8px;
      margin-top: 10px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.5);
    }

    .tab-content.active {
      display: block;
    }

    .movie-title {
      color: var(--accent-color);
      margin-top: 0;
    }

    .movie-info {
      font-size: 0.9em;
      color: var(--text-secondary);
      margin-bottom: 15px;
    }

    p {
      line-height: 1.6;
    }
  </style>
</head>
<body>

  <header>
    <h1>Velozes e Furiosos</h1>
    <p>Guia de filmes e resumos da franquia</p>
  </header>

  <div class="tabs-container">
    <div class="tabs-header">
      <button class="tab-btn active" onclick="openTab(event, 'film1')">Velozes 1</button>
      <button class="tab-btn" onclick="openTab(event, 'film2')">Mais Velozes</button>
      <button class="tab-btn" onclick="openTab(event, 'film3')">Tóquio</button>
      <button class="tab-btn" onclick="openTab(event, 'film4')">Velozes 4</button>
      <button class="tab-btn" onclick="openTab(event, 'film5')">Operation Rio</button>
      <button class="tab-btn" onclick="openTab(event, 'film6')">Velozes 6</button>
      <button class="tab-btn" onclick="openTab(event, 'film7')">Velozes 7</button>
      <button class="tab-btn" onclick="openTab(event, 'film8')">Velozes 8</button>
      <button class="tab-btn" onclick="openTab(event, 'film9')">Velozes 9</button>
      <button class="tab-btn" onclick="openTab(event, 'film10')">Velozes 10</button>
    </div>

    <!-- Conteúdo das Abas -->
    <div id="film1" class="tab-content active">
      <h2 class="movie-title">Velozes e Furiosos (2001)</h2>
      <div class="movie-info">Ano: 2001 | Direção: Rob Cohen</div>
      <p>Um policial disfarçado investiga uma gangue de corredores de rua suspeita de orquestrar assaltos a caminhões de carga. À medida que ele se infiltra no submundo das corridas clandestinas de Los Angeles, precisa decidir onde reside sua verdadeira lealdade.</p>
    </div>

    <div id="film2" class="tab-content">
      <h2 class="movie-title">+ Velozes + Furiosos (2003)</h2>
      <div class="movie-info">Ano: 2003 | Direção: John Singleton</div>
      <p>Após deixar a polícia, o ex-agente Brian O'Conner recomeça a vida em Miami. Para limpar seu histórico, ele aceita uma missão federal para derrubar um poderoso negociante de drogas local com a ajuda de um antigo amigo de infância.</p>
    </div>

    <div id="film3" class="tab-content">
      <h2 class="movie-title">Velozes e Furiosos: Desafio em Tóquio (2006)</h2>
      <div class="movie-info">Ano: 2006 | Direção: Justin Lin</div>
      <p>Um jovem problemático apaixonado por carros é enviado para morar com o pai no Japão para evitar a prisão. Em Tóquio, ele descobre o perigoso estilo de corrida conhecido como drift e precisa aprender a técnica para enfrentar o campeão local.</p>
    </div>

    <div id="film4" class="tab-content">
      <h2 class="movie-title">Velozes e Furiosos 4 (2009)</h2>
      <div class="movie-info">Ano: 2009 | Direção: Justin Lin</div>
      <p>Quando um crime trágico afeta pessoas próximas, um fugitivo e um agente federal reatam sua antiga parceria em uma busca por justiça. Juntos, eles se infiltram em um cartel internacional de drogas que opera na fronteira mexicana.</p>
    </div>

    <div id="film5" class="tab-content">
      <h2 class="movie-title">Velozes e Furiosos 5: Operação Rio (2011)</h2>
      <div class="movie-info">Ano: 2011 | Direção: Justin Lin</div>
      <p>Buscando a liberdade definitiva, a equipe reúne especialistas para realizar um grande assalto contra um empresário corrupto no Rio de Janeiro, enquanto são perseguidos por um implacável agente federal americano.</p>
    </div>

    <div id="film6" class="tab-content">
      <h2 class="movie-title">Velozes e Furiosos 6 (2013)</h2>
      <div class="movie-info">Ano: 2013 | Direção: Justin Lin</div>
      <p>Espalhados pelo mundo após o golpe no Brasil, os membros do grupo são convocados pelo governo para combater uma organização de mercenários altamente treinados que atuam sobre rodas em troca do perdão total de seus crimes.</p>
    </div>

    <div id="film7" class="tab-content">
      <h2 class="movie-title">Velozes e Furiosos 7 (2015)</h2>
      <div class="movie-info">Ano: 2015 | Direção: James Wan</div>
      <p>Após derrotarem seus últimos inimigos, a equipe tenta retornar à vida normal. No entanto, um assassino treinado busca vingança contra o grupo, forçando-os a se unirem mais uma vez para se protegerem.</p>
    </div>

    <div id="film8" class="tab-content">
      <h2 class="movie-title">Velozes e Furiosos 8 (2017)</h2>
      <div class="movie-info">Ano: 2017 | Direção: F. Gary Gray</div>
      <p>Com a equipe tentando levar uma vida tranquila, uma misteriosa cyberterrorista chantageia o líder do grupo, fazendo-o se voltar contra seus próprios amigos. A família precisa se unir como nunca para trazê-lo de volta.</p>
    </div>

    <div id="film9" class="tab-content">
      <h2 class="movie-title">Velozes e Furiosos 9 (2021)</h2>
      <div class="movie-info">Ano: 2021 | Direção: Justin Lin</div>
      <p>A paz de Dom Toretto é interrompida quando ameaças do passado retornam. A equipe precisa enfrentar uma conspiração liderada pelo irmão desaparecido de Dom, um motorista e assassino habilidoso.</p>
    </div>

    <div id="film10" class="tab-content">
      <h2 class="movie-title">Velozes e Furiosos 10 (2023)</h2>
      <div class="movie-info">Ano: 2023 | Direção: Louis Leterrier</div>
      <p>Ao longo de muitas missões, a equipe superou todos os seus adversários. Agora, eles enfrentam o oponente mais letal de suas vidas: uma ameaça que surge das sombras do passado, determinada a destruir tudo e todos que Dom ama.</p>
    </div>
  </div>

  <script>
    function openTab(evt, filmId) {
      const contents = document.querySelectorAll('.tab-content');
      contents.forEach(content => content.classList.remove('active'));

      const buttons = document.querySelectorAll('.tab-btn');
      buttons.forEach(button => button.classList.remove('active'));

      document.getElementById(filmId).classList.add('active');
      evt.currentTarget.classList.add('active');
    }
  </script>
</body>
</html>