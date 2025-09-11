<h1 align="center"> Salut 👋, je suis Ousmane Kane</h1>

<h3 align="center">Passionné par la tech, le développement et l'apprentissage continu</h3>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=KaneOusmane422&label=Profile%20views&color=0e75b6&style=flat" alt="KaneOusmane422" />
</p>

---

### 👨‍💻 À propos de moi

- 🔭 Je travaille sur des projets liés à **la programmation web et aux systèmes intelligents**
- 🌱 J’apprends actuellement **React, Node.js et l'IA appliquée**
- 💬 Pose-moi des questions sur **Python, JavaScript, Git, ou même comment démarrer dans la tech**
- 📫 Me contacter : **okane2858@gmail.com**
- ⚡ Fun fact : J’adore résoudre des casse-têtes tech et bidouiller des projets perso

---

### 🛠️ Langages & outils

<p>
  <img src="https://www.acass.fr/public/img/medium/AdobeStock555641760jpeg_63f87f3d1e718.jpeg/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" />
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
</p>

---

### 📊 Mes stats GitHub

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=KaneOusmane422&show_icons=true&theme=tokyonight" alt="stats KaneOusmane422" />
  <br />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=KaneOusmane422&theme=tokyonight" alt="streak KaneOusmane422" />
</p>

---

### 🔗 Liens utiles

- 💼 [Mon LinkedIn](https://linkedin.com/ousmane-kane
- 🌐 okane2858@gmail.com
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Animation Profil</title>
<style>
  body {
    font-family: 'Poppins', sans-serif;
    background: #0f1724;
    color: #fff;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
    flex-direction: column;
  }
  .animated-text {
    font-size: 2rem;
    font-weight: 600;
    border-right: 2px solid #fff;
    white-space: nowrap;
    overflow: hidden;
    width: 0;
  }
</style>
</head>
<body>

<h1>Ousmane Kane — Développeur</h1>
<div id="text" class="animated-text"></div>

<script>
const text = "Ce profil est en constante évolution...";
const container = document.getElementById('text');
let index = 0;

function typeEffect() {
    if(index < text.length){
        container.style.width = `${index + 1}ch`;
        container.textContent += text.charAt(index);
        index++;
        setTimeout(typeEffect, 100); // vitesse de l'animation
    } else {
        setTimeout(() => { // Réinitialiser l'animation après 2 secondes
            container.textContent = "";
            index = 0;
            typeEffect();
        }, 2000);
    }
}

typeEffect();
</script>

</body>
</html>
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Portfolio — Ousmane Kane</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
<style>
  body {
    margin: 0;
    padding: 0;
    font-family: 'Poppins', sans-serif;
    background: linear-gradient(135deg, #7c3aed, #06b6d4);
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    color: #fff;
    flex-direction: column;
    overflow: hidden;
  }

  h1 {
    font-size: 3rem;
    margin: 0;
    transition: transform 0.3s, color 0.3s;
    cursor: pointer;
    user-select: none;
  }

  h1:hover {
    transform: scale(1.2);
    color: #ffe600;
  }

  button {
    margin-top: 30px;
    padding: 12px 24px;
    font-size: 16px;
    border: none;
    border-radius: 10px;
    background-color: rgba(255,255,255,0.2);
    color: #fff;
    cursor: pointer;
    transition: background-color 0.3s;
  }

  button:hover {
    background-color: rgba(255,255,255,0.5);
  }

  /* Typing effect */
  .typing {
    border-right: 2px solid #fff;
    white-space: nowrap;
    overflow: hidden;
  }
</style>
</head>
<body>

<h1 id="hello" class="typing">Hello World!</h1>
<button onclick="changeMessage()">Clique ici pour découvrir</button>

<script>
const messages = [
    "Hello World!",
    "Bienvenue sur mon portfolio !",
    "Je suis Ousmane Kane — Développeur Web",
    "Projets et créations à découvrir...",
    "Let's code together!"
];

let index = 0;

function typeEffect(text, element, speed = 100) {
    element.textContent = "";
    let i = 0;
    const interval = setInterval(() => {
        if (i < text.length) {
            element.textContent += text.charAt(i);
            i++;
        } else {
            clearInterval(interval);
        }
    }, speed);
}

function changeMessage() {
    const element = document.getElementById('hello');
    typeEffect(messages[index], element);
    index = (index + 1) % messages.length;
}
</script>

</body>
</html>

