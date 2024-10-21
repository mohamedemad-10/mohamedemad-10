<!-- Auto Typing Effect -->
<h1 align="center">
  <span id="title"></span>
</h1>
<h3 align="center">
  <span id="subtitle"></span>
</h3>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=mohamedemad-10&label=Profile%20views&color=0e75b6&style=flat" alt="mohamedemad-10" />
</p>

<p align="center">
  <a href="https://linkedin.com/in/your-linkedin-profile" target="_blank">
    <img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=flat&logo=linkedin&logoColor=white&logoWidth=30" alt="LinkedIn" />
  </a>
  <a href="https://twitter.com/your-twitter-handle" target="_blank">
    <img src="https://img.shields.io/badge/-Twitter-%231DA1F2?style=flat&logo=twitter&logoColor=white&logoWidth=30" alt="Twitter" />
  </a>
  <a href="mailto:mohamedemad.front@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white&logoWidth=30" alt="Email" />
  </a>
</p>

<!-- Rest of your code remains unchanged -->

<!-- JavaScript for Auto-Typing Effect -->
<script>
  const titleText = "Hi 👋, I'm Mohamed Emad";
  const subtitleText = "🚀 A Passionate Frontend Developer from Egypt";
  
  function typeEffect(element, text, delay = 100) {
    let index = 0;
    function type() {
      if (index < text.length) {
        element.innerHTML += text.charAt(index);
        index++;
        setTimeout(type, delay);
      } else {
        setTimeout(() => {
          element.innerHTML = "";
          index = 0;
          type();
        }, 2000); // Delay before rewriting
      }
    }
    type();
  }

  document.addEventListener("DOMContentLoaded", () => {
    const titleElement = document.getElementById("title");
    const subtitleElement = document.getElementById("subtitle");
    typeEffect(titleElement, titleText);
    typeEffect(subtitleElement, subtitleText);
  });
</script>

<style>
  /* Style for typing effect */
  #title, #subtitle {
    border-right: 2px solid;
    white-space: nowrap;
    overflow: hidden;
    display: inline-block;
    animation: blink 0.7s step-end infinite alternate;
  }

  @keyframes blink {
    0% { border-color: transparent; }
    100% { border-color: black; }
  }
</style>
