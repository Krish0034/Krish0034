### Hi there! 👋
<div class='console-container'><span id='text'></span><div class='console-underscore' id='console'>&#95;</div></div>

<script>
  consoleText(['Hello there!', 'Welcome!', 'Nice to meet you!'], 'text', ['tomato', 'rebeccapurple', 'lightblue']);
  
  function consoleText(words, id, colors) {
    if (colors === undefined) colors = ['#fff'];
    var visible = true;
    var con = document.getElementById('console');
    var letterCount = 1;
    var x = 1;
    var waiting = false;
    var target = document.getElementById(id)
    target.setAttribute('style', 'color:' + colors[0])
    window.setInterval(function() {

      if (letterCount === 0 && waiting === false) {
        waiting = true;
        target.innerHTML = words[0].substring(0, letterCount)
        window.setTimeout(function() {
          var usedColor = colors.shift();
          colors.push(usedColor);
          var usedWord = words.shift();
          words.push(usedWord);
          x = 1;
          target.setAttribute('style', 'color:' + colors[0])
          letterCount += x;
          waiting = false;
        }, 1000)
      } else if (letterCount === words[0].length + 1 && waiting === false) {
        waiting = true;
        window.setTimeout(function() {
          x = -1;
          letterCount += x;
          waiting = false;
        }, 1000)
      } else if (waiting === false) {
        target.innerHTML = words[0].substring(0, letterCount)
        letterCount += x;
      }
    }, 120)
    window.setInterval(function() {
      if (visible === true) {
        con.className = 'console-underscore hidden'
        visible = false;

      } else {
        con.className = 'console-underscore'

        visible = true;
      }
    }, 400)
  }
</script>

#### 🚀 About Me

- 🔭 I’m currently working on exciting Flutter projects that push the boundaries of mobile app development.
- 🌱 I’m constantly learning and exploring new technologies in the Flutter ecosystem to stay ahead of the curve.
- 👯 I’m looking to collaborate on open-source Flutter projects and contribute to the vibrant community.
- 🤔 I’m seeking help with advanced state management techniques and animations in Flutter.
- 💬 Ask me about anything related to Flutter, Dart, and mobile app development.
- 📫 How to reach me: [krish.dev@example.com](mailto:kri240799@gmail.com)
- 😄 Pronouns: He/Him
- ⚡ Fun fact: When I'm not coding, you can find me exploring the great outdoors or experimenting with new recipes in the kitchen.

### 🛠️ My Tech Stack

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=flat-square&logo=visual-studio-code&logoColor=white)

### 🌐 Connect with Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/krish0034/)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/_kumar_krishn/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Krish0034)

### 📝 Latest Blog Posts

- [Getting Started with Flutter](https://example.com/blog/getting-started-with-flutter)
- [Understanding State Management in Flutter](https://example.com/blog/state-management-in-flutter)
- [Building Responsive UIs with Flutter](https://example.com/blog/responsive-uis-in-flutter)

### 📊 GitHub Stats

![Krish's GitHub stats](https://github-readme-stats.vercel.app/api?username=Krish0034&show_icons=true&theme=radical)

---

✨ Thank you for visiting my profile! Feel free to explore my repositories and reach out if you want to connect or collaborate. Happy coding! ✨
