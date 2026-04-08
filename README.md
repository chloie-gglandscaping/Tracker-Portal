<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Coast 1Step Portal</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f4f6f8;
      color: #333;
    }

    header {
      position: sticky;
      top: 0;
      background-color: #ffffff;
      z-index: 999;
      border-bottom: 2px solid #2a7ae2;
      box-shadow: 0 2px 6px rgba(0,0,0,0.05);
      padding: 20px 0;
      text-align: center;
    }

    header img.company-logo {
      height: 120px;
      width: auto;
      margin-bottom: 15px;
    }

    #tools {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 50px;
      padding: 15px 0;
    }

    .tool {
      text-align: center;
    }

    .tool a {
      display: inline-block;
      transition: transform 0.2s;
      text-decoration: none;
      color: #333;
    }

    .tool a:hover {
      transform: scale(1.1);
    }

    .tool img {
      height: 80px;
      width: auto;
      display: block;
      margin: 0 auto;
    }

    .tool-name {
      font-size: 14px;
      font-weight: bold;
      color: #2a7ae2;
      margin-top: 4px;
    }

    .search-container {
      padding: 20px;
      text-align: center;
    }

    .search-container input[type="text"] {
      width: 60%;
      max-width: 500px;
      padding: 12px 15px;
      border-radius: 25px;
      border: 1px solid #ccc;
      font-size: 16px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      transition: box-shadow 0.2s, border-color 0.2s;
    }

    .search-container input[type="text"]:focus {
      outline: none;
      border-color: #2a7ae2;
      box-shadow: 0 2px 12px rgba(42,122,226,0.3);
    }

    table {
      width: 90%;
      margin: 20px auto 50px auto;
      border-collapse: collapse;
      background-color: #ffffff;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 4px 10px rgba(0,0,0,0.05);
    }

    th, td {
      padding: 14px 12px;
      text-align: left;
      border-bottom: 1px solid #ddd;
    }

    th {
      background-color: #2a7ae2;
      color: white;
      font-weight: bold;
    }

    tr:nth-child(even) {
      background-color: #f9f9f9;
    }

    tr:hover {
      background-color: #e0e7ff;
    }

    td.category {
      font-weight: bold;
      color: #2a7ae2;
    }

    a {
      color: #2a7ae2;
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    @media (max-width: 768px) {
      #tools {
        gap: 30px;
      }
      .tool img {
        height: 60px;
      }
    }

    @media (max-width: 480px) {
      #tools {
        flex-direction: column;
        gap: 20px;
      }
      .tool img {
        height: 70px;
      }
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <img src="https://i.imgur.com/gFFL080.png" alt="Company Logo" class="company-logo">
    <div id="tools">
      <div class="tool">
        <a href="https://track.onestepgps.com/v3/ux/map/device" target="_blank" title="1Step GPS">
          <img src="https://i.imgur.com/YkcnASY.jpeg" alt="1Step GPS Logo">
          <div class="tool-name">1Step GPS</div>
        </a>
      </div>
      <div class="tool">
        <a href="https://portal.coastpay.com/transactions/iauth_1TJaUlKrLGv3Il3bK6579GkB" target="_blank" title="Coast Manager">
          <img src="https://i.imgur.com/hzJmEvU.png" alt="Coast Manager Logo">
          <div class="tool-name">Coast Manager</div>
        </a>
      </div>
      <div class="tool">
        <a href="https://my.golmn.com/lmn/" target="_blank" title="LMN">
          <img src="https://i.imgur.com/0ZoNM0S.png" alt="LMN Logo">
          <div class="tool-name">LMN</div>
        </a>
      </div>
      <div class="tool">
        <a href="https://accounts.intuit.com/app/sign-in?app_group=QBO&asset_alias=Intuit.accounting.core.qbowebapp" target="_blank" title="QuickBooks">
          <img src="https://i.imgur.com/Ki2MRH0.png" alt="QuickBooks Logo">
          <div class="tool-name">QuickBooks</div>
        </a>
      </div>
      <div class="tool">
        <a href="https://app-na2.hubspot.com/user-guide/244154328?via=home" target="_blank" title="HubSpot">
          <img src="https://i.imgur.com/Qzzj8tw.png" alt="HubSpot Logo">
          <div class="tool-name">HubSpot</div>
        </a>
      </div>
    </div>
  </header>

  <!-- Search -->
  <div class="search-container">
    <input type="text" id="searchInput" onkeyup="searchTable()" placeholder="Search links or descriptions...">
  </div>

  <!-- Table -->
  <table id="linksTable">
    <thead>
      <tr>
        <th>Category</th>
        <th>Link</th>
        <th>Description</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td class="category">Expenses</td>
        <td><a href="https://docs.google.com/spreadsheets/d/1dt39MEvJ1oO9jyiwjb3_AIUMwIuIqTW0GVgTzTsqvKQ/edit?gid=0#gid=0" target="_blank">Materials Expense Sheet</a></td>
        <td>Track all material expenses for projects</td>
      </tr>
      <tr>
        <td class="category">Timesheets</td>
        <td><a href="https://docs.google.com/forms/u/0/d/e/1FAIpQLScJaR6RJFuPLQvtwfEboczQgcUbpAlmkQGp_a-unWdkdoq6aw/formResponse" target="_blank">Timesheet Review</a></td>
        <td>Review employee timesheet submissions</td>
      </tr>
      <tr>
        <td class="category">Clients</td>
        <td><a href="https://docs.google.com/spreadsheets/d/19DC2_6n3iP3621yzsnkj1ihSgDk_FyvDyhy8IxyXsCE/edit?gid=1366508085#gid=1366508085" target="_blank">Active Client List</a></td>
        <td>List of all active clients</td>
      </tr>
      <tr>
        <td class="category">Field Performance</td>
        <td><a href="https://docs.google.com/spreadsheets/d/1zLpcjFFj3GgFilmGPmKHdlQxWkf6cruNSnEGUS7U9-I/edit?gid=981445567#gid=981445567" target="_blank">Field Performance</a></td>
        <td>Track crew and field performance metrics</td>
      </tr>
    </tbody>
  </table>

  <script>
    function searchTable() {
      const input = document.getElementById("searchInput").value.toLowerCase();
      const table = document.getElementById("linksTable");
      const rows = table.getElementsByTagName("tr");

      for (let i = 1; i < rows.length; i++) {
        let cells = rows[i].getElementsByTagName("td");
        let match = false;
        for (let j = 0; j < cells.length; j++) {
          if (cells[j].innerText.toLowerCase().includes(input)) {
            match = true;
            break;
          }
        }
        rows[i].style.display = match ? "" : "none";
      }
    }
  </script>

</body>
</html>
