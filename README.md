# Shreyansh_Kumar_18

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Career Guidance</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
        }
        body {
            background-color: #121212;
            color: white;
            text-align: center;
            overflow: hidden;
        }
        header {
            background: #1c1c1c;
            padding: 15px;
            font-size: 24px;
            font-weight: bold;
            color: #ff4757;
        }
        .container {
            width: 100vw;
            height: 100vh;
            display: flex;
            transition: transform 0.5s ease-in-out;
        }
        .page {
            width: 100vw;
            height: 100vh;
            flex-shrink: 0;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }
        .btn {
            background: #ff4757;
            color: white;
            padding: 15px;
            border: none;
            margin: 10px;
            cursor: pointer;
            font-size: 18px;
            border-radius: 5px;
            transition: 0.3s;
        }
        .btn:hover {
            background: #e84118;
        }
        input {
            padding: 10px;
            margin: 10px;
            width: 80%;
            font-size: 16px;
        }
        iframe {
            width: 80%;
            height: 400px;
            border: none;
        }
    </style>
</head>
<body>

<header>Career Guidance</header>

<div class="container">
    <!-- Page 1: UG/PG Selection -->
    <section class="page">
        <h2>Are you a?</h2>
        <button class="btn" onclick="nextPage()">Undergraduate</button>
        <button class="btn" onclick="nextPage()">Postgraduate</button>
        <button class="btn" onclick="nextPage()">Student</button>
    </section>

    <!-- Page 2: Login -->
    <section class="page">
        <h2>Login</h2>
        <input type="email" placeholder="Enter Email" required>
        <input type="password" placeholder="Enter Password" required>
        <button class="btn" onclick="nextPage()">Login</button>
    </section>

    <!-- Page 3: Welcome (Styled like reference image) -->
    <section class="page">
        <h2>Welcome Back, Alex</h2>
        <p>Your career journey continues today!</p>
        <div>
            <button class="btn">Personalised Skill Development</button>
            <button class="btn">Career Path Alignment</button>
            <button class="btn">Progress Tracking</button>
            <button class="btn">Industry Aligned Assessment</button>
            <button class="btn">Scalable/Peer Learning</button>
        </div>
        <button class="btn" onclick="nextPage()">Continue</button>
    </section>

    <!-- Page 4: Chatbot -->
    <section class="page">
        <h2>Career Chatbot</h2>
        <iframe src="https://landbot.online/v3/H-2832591-B3Q8NY0QX79IIJWZ/index.html"></iframe>
        <button class="btn" onclick="nextPage()">Next</button>
    </section>

    <!-- Page 5: Real-Time Mentorship -->
    <section class="page">
        <h2>Select a Time Slot for Mentorship</h2>
        <button class="btn">10:00 AM - 11:00 AM</button>
        <button class="btn">2:00 PM - 3:00 PM</button>
        <button class="btn">5:00 PM - 6:00 PM</button>
        <button class="btn">8:00 PM - 9:00 PM</button>
    </section>
</div>

<script>
    let page = 0;
    function nextPage() {
        page++;
        document.querySelector(".container").style.transform = `translateX(-${page * 100}vw)`;
    }
</script>

</body>
</html>

