<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Евгений & Алёна | 14.06.2025</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Montserrat:wght@300;400&display=swap" rel="stylesheet">
    <style>
        :root {
            --gold: #d4af37;
            --rose: #f8d7da;
            --dark: #333;
        }
        
        body {
            font-family: 'Montserrat', sans-serif;
            margin: 0;
            padding: 0;
            background: #fff9fb;
            color: var(--dark);
            overflow-x: hidden;
        }
        
        .heart {
            color: #ff6b6b;
        }
        
        header {
            background: linear-gradient(rgba(0,0,0,0.3), rgba(0,0,0,0.3)), url('https://images.unsplash.com/photo-1519225421980-715cb0215aed?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
        }
        
        h1 {
            font-family: 'Playfair Display', serif;
            font-size: 4rem;
            margin: 0;
            animation: fadeIn 2s;
        }
        
        .date {
            font-size: 1.8rem;
            margin: 20px 0;
            letter-spacing: 3px;
            animation: fadeIn 2s 0.5s both;
        }
        
        .names {
            display: flex;
            align-items: center;
            gap: 20px;
            margin-bottom: 30px;
            animation: fadeIn 2s 1s both;
        }
        
        .names span {
            font-size: 2rem;
        }
        
        .timer {
            display: flex;
            gap: 15px;
            margin: 40px 0;
            animation: fadeIn 2s 1.5s both;
        }
        
        .timer-item {
            background: rgba(255,255,255,0.2);
            padding: 15px;
            border-radius: 5px;
            min-width: 80px;
        }
        
        .timer-number {
            font-size: 2rem;
            font-weight: bold;
        }
        
        section {
            padding: 80px 20px;
            max-width: 1000px;
            margin: 0 auto;
        }
        
        .section-title {
            font-family: 'Playfair Display', serif;
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 50px;
            color: var(--gold);
        }
        
        .program {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 30px;
        }
        
        .program-item {
            flex: 1;
            min-width: 250px;
            text-align: center;
            padding: 30px;
            background: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        
        .program-item:hover {
            transform: translateY(-10px);
        }
        
        .program-item h3 {
            color: var(--gold);
        }
        
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 40px;
        }
        
        .gallery img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px;
            transition: transform 0.3s;
            cursor: pointer;
        }
        
        .gallery img:hover {
            transform: scale(1.05);
        }
        
        .rsvp {
            background: var(--rose);
            padding: 50px 20px;
            text-align: center;
        }
        
        .rsvp-form {
            max-width: 500px;
            margin: 0 auto;
        }
        
        .form-group {
            margin-bottom: 20px;
            text-align: left;
        }
        
        input, textarea, select {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-family: inherit;
        }
        
        button {
            background: var(--gold);
            color: white;
            border: none;
            padding: 15px 40px;
            font-size: 1rem;
            border-radius: 50px;
            cursor: pointer;
            transition: background 0.3s;
        }
        
        button:hover {
            background: #c9a227;
        }
        
        footer {
            text-align: center;
            padding: 30px;
            background: var(--dark);
            color: white;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }
            
            .names {
                flex-direction: column;
                gap: 5px;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Евгений <span class="heart">❤</span> Алёна</h1>
        <div class="date">14 ИЮНЯ 2025</div>
        <div class="names">
            <span>Евгений</span>
            <span class="heart">❤</span>
            <span>Алёна</span>
        </div>
        <div class="timer" id="timer">
            <div class="timer-item">
                <div class="timer-number" id="days">00</div>
                <div>дней</div>
            </div>
            <div class="timer-item">
                <div class="timer-number" id="hours">00</div>
                <div>часов</div>
            </div>
            <div class="timer-item">
                <div class="timer-number" id
