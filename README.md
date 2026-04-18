<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Green Garden Portal</title>

<style>
body {
  margin: 0;
  font-family: Arial;
  background: #eef2f6;
}

/* HEADER */
header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: white;
  padding: 8px 16px;
  border-bottom: 2px solid #2a7ae2;
  position: relative;
}

.company-logo { height: 150px; }

.tools-wrapper {
  flex: 1;
  display: flex;
  justify-content: center;
}

#tools {
  display: flex;
  gap: 12px;
}

.tool a {
  width: 85px;
  height: 95px;
  background: white;
  border-radius: 12px;
  display: flex;
  align-items: center;
  justify-content: center;
  text-decoration: none;
  box-shadow: 0 2px 6px rgba(0,0,0,0.08);
}

.tool img {
  height: 45px;
  animation: bounce 1.6s infinite;
}

@keyframes bounce {
  0%{transform:translateY(0)}
  20%{transform:translateY(-10px)}
  40%{transform:translateY(0)}
  60%{transform:translateY(-6px)}
  100%{transform:translateY(0)}
}

/* ✅ IMPROVED CLOCK (UPDATED) */
.clock {
  position: absolute;
  right: 15px;
  top: 10px;
  background: linear-gradient(135deg, #1f4fa3, #2a7ae2);
  color: white;
  padding: 10px 14px;
  border-radius: 14px;
  font-size: 13px;
  font-weight: bold;
  box-shadow: 0 4px 10px rgba(0,0,0,0.2);
  letter-spacing: 0.5px;
}

/* MAIN */
.container {
  max-width: 1100px;
  margin: 20px auto;
  padding: 10px;
}

h2 {
  text-align: center;
  color: #2a7ae2;
}

#search {
  width: 100%;
  padding: 12px;
  border-radius: 25px;
  border: 1px solid #ccc;
}

/* CATEGORY */
.category {
  margin-top: 18px;
}

.cat-title {
  background: #2a7ae2;
  color: white;
  padding: 10px;
  cursor: pointer;
  border-radius: 8px;
}

/* LINKS */
.links {
  padding: 10px;
}

/* LINK CARD */
.link {
  display: block;
  background: white;
  padding: 12px;
  margin: 8px 0;
  border-radius: 10px;
  text-decoration: none;
  color: #333;
  box-shadow: 0 2px 6px rgba(0,0,0,0.08);
  transition: 0.2s;
}

.link:hover {
  transform: translateY(-3px);
}

/* STAR */
.star {
  float: right;
  color: gold;
  cursor: pointer;
}

</style>
</head>

<body>

<header>

<img class="company-logo" src="https://i.imgur.com/gFFL080.png">

<div class="tools-wrapper">
  <div id="tools">

    <div class="tool"><a href="https://my.golmn.com/lmn/"><img src="https://i.imgur.com/0ZoNM0S.png"></a></div>
    <div class="tool"><a href="https://track.onestepgps.com/v3/ux/map/device"><img src="https://i.imgur.com/YkcnASY.jpeg"></a></div>
    <div class="tool"><a href="https://portal.coastpay.com/"><img src="https://i.imgur.com/hzJmEvU.png"></a></div>
    <div class="tool"><a href="https://accounts.intuit.com/"><img src="https://i.imgur.com/Ki2MRH0.png"></a></div>
    <div class="tool"><a href="https://app-na2.hubspot.com/"><img src="https://i.imgur.com/Qzzj8tw.png"></a></div>
    <div class="tool"><a href="https://www.chase.com/"><img src="https://i.imgur.com/gR74mO9.png"></a></div>
    <div class="tool"><a href="https://ring.com/users/sign_in"><img src="https://i.imgur.com/eHgyJTI.png"></a></div>

  </div>
</div>

<div class="clock" id="clock"></div>

</header>

<div class="container">

<h2>Company Portal</h2>

<input id="search" onkeyup="search()" placeholder="Search everything...">

<!-- 🧠 ADMIN -->
<div class="category">
<div class="cat-title" onclick="toggle(this)">🧠 Admin / SOP / Guides</div>
<div class="links">

<a class="link" href="https://docs.google.com/document/d/10vbwLFoDObrQIzl7QZE3KzEiUEK2AeoaBOKQ1rlDGvw/edit" target="_blank">Employee Guide - Admin Team</a>

<a class="link" href="https://docs.google.com/document/d/1of6N9AWggZ96SlNE06XaQDO60uJurntYsoTBfWXglE8/edit" target="_blank">Employee Guide - Field Crews Only</a>

<a class="link" href="https://docs.google.com/document/d/1S5o2luP-g-nAg8HyIs_JKSX3GsWJKSqHnVTbov0LYbs/edit" target="_blank">Comms SOP</a>

<a class="link" href="https://docs.google.com/document/d/11aonoolHgvSB85LIAJtOrtdXP18LZea4sw8aN3Nocy4/edit" target="_blank">Sales Process SOP</a>

<a class="link" href="https://docs.google.com/document/d/1o8wUuIpxmzmTFhTzQC_rNl9-nTFwTQVQ9DndMfsJHwQ/edit" target="_blank">New Hire SOP</a>

<a class="link" href="https://docs.google.com/document/d/1hpDl9r75jNz25nmov2zI5dYjvUHZBvFcxNlav_OXeb4/edit" target="_blank">Field Crew Weekly Meetings SOP</a>

</div>
</div>

<!-- 📊 FORMS -->
<div class="category">
<div class="cat-title" onclick="toggle(this)">📊 Forms / Reporting</div>
<div class="links">

<a class="link" href="https://docs.google.com/forms/d/e/1FAIpQLSd-JZKnXuDj_Rdc2-gtrD7pWdMcpqiFjBEdlxniRVHVuU3BbQ/viewform" target="_blank">EOD Report</a>

<a class="link" href="https://docs.google.com/forms/d/e/1FAIpQLScJaR6RJFuPLQvtwfEboczQgcUbpAlmkQGp_a-unWdkdoq6aw/viewform" target="_blank">Timesheet Review</a>

<a class="link" href="https://docs.google.com/forms/d/1b78G6rkZJcVEFv9fb9vtRITcMvsW9wmw7fVN4zi4yTY/edit" target="_blank">Field Attendance Tracker</a>

</div>
</div>

<!-- 📈 OPERATIONS -->
<div class="category">
<div class="cat-title" onclick="toggle(this)">📈 Operations</div>
<div class="links">

<a class="link" href="https://docs.google.com/spreadsheets/d/19DC2_6n3iP3621yzsnkj1ihSgDk_FyvDyhy8IxyXsCE/edit" target="_blank">Active Client List</a>

<a class="link" href="https://docs.google.com/spreadsheets/d/19fFHogL9xT2_IWSGF92d0HhT02oE5qAnFv9tLZBpIi4/edit" target="_blank">Fleet Tracker</a>

<a class="link" href="https://docs.google.com/spreadsheets/d/10xpcopHNTJcFxCGs9ZNuUnFA3ekVJVcUlJ_gl9OGQhw/edit" target="_blank">Invoice Master</a>

<a class="link" href="https://docs.google.com/spreadsheets/d/1biEo0sPwOQE61FXNb5z27H9V2p3Xwi2VGTgQw2mo_ew/edit" target="_blank">Headcount Master</a>

<a class="link" href="https://docs.google.com/spreadsheets/d/1CGRRUNN9QIv60cWESrEx2IgCSIAisvcbyn2iyHZ7FfQ/edit" target="_blank">Scorecard Tracker</a>

<a class="link" href="https://docs.google.com/spreadsheets/d/1zLpcjFFj3GgFilmGPmKHdlQxWkf6cruNSnEGUS7U9-I/edit" target="_blank">Field Performance Tracker</a>

</div>
</div>

<!-- 📁 STORAGE -->
<div class="category">
<div class="cat-title" onclick="toggle(this)">📁 Storage</div>
<div class="links">

<a class="link" href="https://drive.google.com/drive/folders/1EXGz9Afrt5h2XYA5LWnwXfhRo55smrgy" target="_blank">Billing Folder</a>

</div>
</div>

</div>

<script>

/* CLOCK */
function updateClock(){
  const now = new Date();

  const options = {
    timeZone: "America/Los_Angeles",
    hour: "2-digit",
    minute: "2-digit",
    second: "2-digit",
    hour12: true
  };

  const time = new Intl.DateTimeFormat("en-US", options).format(now);

  document.getElementById("clock").innerHTML =
    "Seattle • " + time;
}

setInterval(updateClock, 1000);
updateClock();

/* SEARCH */
function search(){
  let v=document.getElementById("search").value.toLowerCase();
  document.querySelectorAll(".link").forEach(e=>{
    e.style.display=e.innerText.toLowerCase().includes(v)?"block":"none";
  });
}

/* COLLAPSE */
function toggle(el){
  let box=el.nextElementSibling;
  box.style.display=(box.style.display==="none")?"block":"none";
}

</script>

</body>
</html>
