<!DOCTYPE html>
<html>
<head>
<style>
  .tab {
    overflow: hidden;
    background-color: #f2f2f2;
  }

  .tab button {
    background-color: #d3d3d3;
    float: left;
    border: none;
    outline: none;
    cursor: pointer;
    padding: 14px 16px;
    transition: 0.3s;
  }

  .tab button:hover {
    background-color: #ddd;
  }

  .tab button.active {
    background-color: #ff69b4;
    color: white;
  }

  .tabcontent {
    display: none;
    padding: 6px 12px;
    border-top: none;
  }

  .profile {
    font-family: 'cursive';
    text-align: center;
    color: #ff69b4;
  }

  .image {
    float: right;
  }
</style>
</head>
<body>

<div class="tab">
  <button class="tablinks" onclick="openTab(event, 'Profile')">Profile</button>
  <button class="tablinks" onclick="openTab(event, 'Stats')">Stats</button>
</div>

<div id="Profile" class="tabcontent">
  <div class="profile">
    <img src="https://tinyurl.com/yp5eqvz4">
    <h1>👧🏻 Hi, I'm Tharushi Ranathunga</h1>
    <h3>👨‍🎓 Student | ✍️ Passionate Coder | 🌟 Learning & Growing</h3>
    <p>"Coding is my canvas, and I paint my dreams with code."</p>
    <h4>How to reach me: <a href="mailto:work.tharushiranathunga@gmail.com" style="text-decoration: none; color: #ff69b4;">work.tharushiranathunga@gmail.com</a></h4>
  </div>
  <div class="image">
    <img align="right" alt="Coding" width="400" src="https://i.scdn.co/image/ab67706c0000da84edcece3a396ce1f51fe40385">
  </div>
</div>

<div id="Stats" class="tabcontent">
  <h4>Languages and Tools:</h4>
  <p>
    <a href="https://www.figma.com/" target="_blank" rel="noreferrer">
      <img src="https://www.vectorlogo.zone/logos/figma/figma-icon.svg" alt="figma" width="40" height="40"/>
    </a>
    <!-- Add more icons here -->
  </p>
  <p><img src="https://github-readme-stats.vercel.app/api/top-langs?username=tharushiranathunga&show_icons=true&locale=en&layout=compact" alt="tharushiranathunga" /></p>
  <p><img src="https://github-readme-stats.vercel.app/api?username=tharushiranathunga&show_icons=true&locale=en" alt="tharushiranathunga" /></p>
  <p><img src="https://github-readme-streak-stats.herokuapp.com/?user=tharushiranathunga&" alt="tharushiranathunga" /></p>
</div>

<script>
function openTab(evt, tabName) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(tabName).style.display = "block";
  evt.currentTarget.className += " active";
}
</script>

</body>
</html>
