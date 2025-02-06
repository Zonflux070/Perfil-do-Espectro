<!--doctype html-->
<html lang="pt-BR"> 
  <head> 
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Perfil do Everso</title>
    <style>
      /* Estilo Geral */
body {
  color: #FFFFFF;
  font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
  background-color: #000000;
  margin: 0px;
  padding: 0px;
}
/* Barra de Menu*/
.menu {
  position: fixed;
  top: 0px;
  left: -60%;
  width: 60%;
  height: 100%;
  background-color: #FF4747CC;
  transition: 0.3s;
}
.menu ul {
  list-style: none;
  padding: 0px;
}
.menu li {
  text-align: center;
  padding: 15px;
}
.menu a {
  color: #FFFFFF;
  font-size: 18px;
  text-decoration: none;
}
/* Cabeçalho */
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: #FFFFFF;
  width: 100%;
  background: #E41A1A;
  margin: 0px;
  padding: 0px;
}
.logo {
  width: 40px;
  height: 40px;
  border: 1px solid #FFFFFFB8;
  border-radius: 30%;
}
.menu-icon {
  font-size: 30px;
  cursor: pointer;
}
/* Corpo Principal*/
main {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
  margin: 0px;
  padding: 0px;
}
h1, h2, h3 {
  font-family: 'Times New Roman', Times, serif;
}
.descricao {
  text-align: justify;
}
.detalhe {
  text-align: left;
}
section {
  width: 100%;
  margin: 0px;
  padding: 0px;
  background: #000000;
  text-align: center;
}
.imagem img {
  width: 300px;
  height: 300px;
  border-radius: 50%;
}
.imagem a {
  font-size: 18px;
  color: #FFFFFF;
}
.icon img {
  width: 30px;
  height: 30px;
  margin: 5px;
}
/* Rodapé */
footer {
  font-family: monospace;
  font-size: 10px;
  margin: 0px;
  padding: 0px;
  background: #7A2222D4;
  color: #FFFFFF;
  width: 100%;
  text-align: center;
}
.perna {
  font-size: 18px;
  color: #FFFFFF;
}
/* Responsividade */
@media (min-width: 768px) {
  main {
    flex-direction: row;
    justify-content: space-around;
  }
  .menu {
    width: 30%;
    left: -30%;
  }
}
    </style>
  </head> 
  <body> 
    <!--Barra de Menu-->
    <nav id="menu" class="menu">
      <ul>
        <li><a href="#">Pág 1</a></li>
        <li><a href="#">Pág 2</a></li>
        <li><a href="#">Pág 3</a></li>
      </ul>
    </nav>
    <!--Cabeçalho-->
    <header>
      <div>
        <img class="logo" src="playlistCropperBoomPlayer.jpg">
      </div>
      <div class="menu-icon" onclick="toggleMenu()">☰</div>
    </header>
    <!--Corpo Principal -->
    <main>
      <!--1ª Secção -->
      <section class="descricao">
        <h1>Perfil</h1>
        <p>Everso: O Herói que Renasceu das Cinzas</p>
        <h2>Sobre Everso</h2>
        <p>Espectro, o carismático e empático guardião de Telethra, era a personificação da justiça e da ordem. Seu espírito inabalável inspirava esperança, até que a verdade foi revelada: ele não era um ser comum, mas sim um robô. E, diante daqueles que jurou proteger, foi impiedosamente destruído.<br /><br />Porém, dos destroços e da traição, algo novo emergiu. Espectro renasceu como Everso, um herói implacável, violento e marcado pelo orgulho. Seu senso de justiça foi distorcido pela dor da perda, e agora ele caminha entre a redenção e a ruína. No entanto, dentro desse guerreiro endurecido, a essência de Espectro ainda luta para resistir à escuridão que ameaça consumi-lo.</p>
      </section>
      <!--2ª secção -->
      <section class="imagem">
        <img src="The Red Hood Rises 🌩️ A stormy night in Gotham, Jason Todd takes justice into his own hands_ 🔥.jpeg" alt="everso">
        <a href="https://zonflux070.github.io/Z-nflux---Espectro/">Espectro</a>
      </section>
      <!--3ª secção -->
      <section class="detalhe">
        <h3>Detalhes</h3>
        <p><strong>Nome:</strong><br />Everso</p><br />
        <p><strong>Habilidade:</strong><br />Resistência e agilidade</p><br />
        <p><strong>Localização:</strong><br />Telethra</p><br />
        <div>
          <a class="icon" href="#"><img src="Evil octopus vector image on VectorStock.jpeg"></a>
        </div>
      </section>
    </main>
      <!--Rodape-->
    <footer>
        <p>A você, visitante, nosso mais sincero agradecimento por embarcar nesta jornada fascinante sobre o Espectro. Sua curiosidade e dedicação nos motivam a continuar explorando os mistérios deste universo tão único. Esperamos que cada secção lida tenha despertado sua imaginação e lhe oferecido momentos de reflexão e inspiração.</p>
        <a class="perna" href="#">Mecânico</a>
        <p>© 2025 Universo Zônflux. Todos os direitos reservados.</p>
    </footer>
  
 <script>
   function toggleMenu() {
  const menu = document.getElementById('menu');
  if (menu.style.left === "0px") {
    menu.style.left = "-60%";
    document.removeEventListener("click", closeMenuOnClickOutside);
  } else {
    menu.style.left = "0px";
    setTimeout(() => {
      document.addEventListener("click", closeMenuOnClickOutside);
    }, 100);
  }
}

function closeMenuOnClickOutside(event) {
  const menu = document.getElementById('menu');
  const menuIcon = document.querySelector(".menu-icon");

  if (!menu.contains(event.target) && !menuIcon.contains(event.target)) {
    menu.style.left = "-60%";
    document.removeEventListener("click", closeMenuOnClickOutside);
  }
      }
 </script>
  </body>
</html>
