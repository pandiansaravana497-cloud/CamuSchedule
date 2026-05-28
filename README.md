# Ex08 CAMU Schedule using Bootstrap
## Date:

## AIM:
To design a responsive and visually appealing CAMU Schedule using Bootstrap.

## DESIGN STEPS:
### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Add the Bootstrap CDN link inside the <head> section.

### Step 5:
Insert a table element with Bootstrap table classes.

### Step 6:
Construct the complete table.

### Step 7:
Add a header/footer displaying copyright information.

### Step 8:
Publish the website in the LocalHost.

## PROGRAM :
~~~
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Saveetha Timetable</title>

  <link rel="stylesheet"
  href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"/>

  <style>

    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:Arial, Helvetica, sans-serif;
    }

    body{
      display:flex;
      background:#f5f7fb;
    }

    /* SIDEBAR */

    .sidebar{
      width:280px;
      height:100vh;
      background:#fff;
      border-right:1px solid #ddd;
      padding:20px 15px;
    }

    .logo{
      text-align:center;
      margin-bottom:40px;
    }

    .logo img{
      width:180px;
    }

    .logo h2{
      font-size:18px;
      margin-top:10px;
      color:#1e293b;
    }

    .logo p{
      color:#64748b;
      margin-top:5px;
    }

    .menu{
      margin-top:30px;
    }

    .menu a{
      display:flex;
      align-items:center;
      gap:15px;
      text-decoration:none;
      color:#2563eb;
      padding:15px 18px;
      border-radius:12px;
      margin-bottom:10px;
      font-size:18px;
      transition:0.3s;
    }

    .menu a:hover{
      background:#dbeafe;
    }

    .active{
      background:#dbeafe;
    }

    /* MAIN */

    .main{
      flex:1;
      padding:30px;
    }

    .top{
      display:flex;
      justify-content:space-between;
      align-items:flex-start;
      margin-bottom:30px;
    }

    .title h1{
      font-size:50px;
      color:#111827;
    }

    .title h2{
      color:#2563eb;
      margin-top:10px;
      font-size:34px;
    }

    .buttons{
      display:flex;
      gap:15px;
    }

    .btn{
      padding:12px 28px;
      border-radius:30px;
      border:2px solid #2563eb;
      background:white;
      color:#2563eb;
      cursor:pointer;
      font-size:18px;
    }

    .btn.gray{
      border:1px solid #cbd5e1;
      color:#475569;
    }

    /* CARD */

    .card{
      background:white;
      border-radius:20px;
      overflow:hidden;
      border:1px solid #ddd;
    }

    .card-header{
      padding:25px 30px;
      border-bottom:1px solid #e5e7eb;
      display:flex;
      justify-content:space-between;
      align-items:center;
    }

    .card-header h2{
      font-size:42px;
      color:#111827;
    }

    .arrows{
      font-size:25px;
      color:#1e293b;
    }

    /* SUBJECT */

    .subject{
      padding:28px 30px;
      border-bottom:1px solid #e5e7eb;
      display:flex;
      justify-content:space-between;
      align-items:flex-start;
    }

    .subject-left h3{
      font-size:28px;
      margin-bottom:12px;
      color:#111827;
    }

    .teacher{
      color:#2563eb;
      font-size:24px;
    }

    .subject-right{
      text-align:right;
    }

    .time{
      font-size:28px;
      color:#475569;
      margin-bottom:10px;
    }

    .duration{
      color:#64748b;
      font-size:22px;
    }

  </style>

</head>

<body>

  <!-- SIDEBAR -->

  <div class="sidebar">

    <div class="logo">
      <img src="assets/images/saveetha-logo.png">

      <h2>Saveetha Engineering College</h2>
      <p>(Autonomous)</p>
    </div>

    <div class="menu">

      <a href="#">
        <i class="fa-solid fa-chart-column"></i>
        Reports
      </a>

      <a href="#">
        <i class="fa-solid fa-chart-line"></i>
        Progress Report
      </a>

      <a href="#">
        <i class="fa-solid fa-list-check"></i>
        Assessments
      </a>

      <a href="#">
        <i class="fa-solid fa-calendar"></i>
        Holidays
      </a>

      <a href="#" class="active">
        <i class="fa-solid fa-clock"></i>
        Timetable
      </a>

      <a href="#">
        <i class="fa-solid fa-book"></i>
        Teaching Content
      </a>

      <a href="#">
        <i class="fa-solid fa-plane"></i>
        Leave
      </a>

    </div>

  </div>

  <!-- MAIN CONTENT -->

  <div class="main">

    <div class="top">

      <div class="title">
        <h1>Timetable</h1>
        <h2>EVEN-JUNIOR | 2025-2026</h2>
      </div>

      <div class="buttons">
        <button class="btn gray">Today</button>
        <button class="btn">Weekly Schedule</button>
      </div>

    </div>

    <!-- TIMETABLE CARD -->

    <div class="card">

      <div class="card-header">
        <h2>28 May 2026</h2>

        <div class="arrows">
          &lt;&nbsp;&nbsp;&gt;
        </div>
      </div>

      <!-- SUBJECT -->

      <div class="subject">

        <div class="subject-left">
          <h3>Introduction to Machine Learning (19AI410)</h3>
          <div class="teacher">PRIYADHARSINI S</div>
        </div>

        <div class="subject-right">
          <div class="time">8:00 AM - 9:00 AM</div>
          <div class="duration">60 min</div>
        </div>

      </div>

      <div class="subject">

        <div class="subject-left">
          <h3>Introduction to Machine Learning (19AI410)</h3>
          <div class="teacher">PRIYADHARSINI S</div>
        </div>

        <div class="subject-right">
          <div class="time">9:00 AM - 10:00 AM</div>
          <div class="duration">60 min</div>
        </div>

      </div>

      <div class="subject">

        <div class="subject-left">
          <h3>Introduction to Machine Learning (19AI410)</h3>
          <div class="teacher">PRIYADHARSINI S</div>
        </div>

        <div class="subject-right">
          <div class="time">10:00 AM - 11:00 AM</div>
          <div class="duration">60 min</div>
        </div>

      </div>

      <div class="subject">

        <div class="subject-left">
          <h3>Introduction to Machine Learning (19AI410)</h3>
          <div class="teacher">PRIYADHARSINI S</div>
        </div>

        <div class="subject-right">
          <div class="time">11:00 AM - 12:00 PM</div>
          <div class="duration">60 min</div>
        </div>

      </div>

    </div>

  </div>

</body>
</html>
~~~


## OUTPUT:

<img width="1768" height="897" alt="image" src="https://github.com/user-attachments/assets/b21e59f9-175d-46d0-bb0b-8f0fa4d36eed" />



## RESULT:
A responsive and visually appealing CAMU Schedule web page using Bootstrap is designed successfully.
