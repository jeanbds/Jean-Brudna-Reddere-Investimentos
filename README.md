<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jean Carlo Brudna - Assessor de Investimentos</title>
    <style>
        body {
            font-family: 'Segoe UI', Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background: linear-gradient(135deg, #155083 0%, #1a2b5a 100%);
            background-image: url('Reddere logo.png'); /* Logo da Reddere como fundo */
            background-size: cover;
            background-position: center;
        }

        .card {
            background: rgba(255, 255, 255, 0.95);
            border-radius: 16px;
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.2);
           width: 90%;
            max-width: 400px;
            padding: 30px;
            text-align: center;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.3);
            margin-left: 50px; /* Adiciona um espaço de 50px à esquerda, movendo o cartão para a direita */
}
                     

        }

        h1 {
            font-size: 26px;
            color: #1a2b5a;
            margin: 15px 0 5px;
            font-weight: 600;
        }

        h2 {
            font-size: 18px;
            color: #4a5568;
            margin: 0 0 20px;
            font-weight: 500;
        }

        .contact-info {
            margin: 25px 0;
        }

        .contact-info p {
            margin: 12px 0;
            font-size: 16px;
            color: #2d3748;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
        }

        a {
            color: #2b6cb0;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        a:hover {
            color: #1a4a8a;
            text-decoration: underline;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 25px;
        }

        .social-links a {
            background: #1a2b5a;
            color: white;
            padding: 12px 25px;
            border-radius: 8px;
            font-weight: 500;
            display: flex;
            align-items: center;
            gap: 8px;
            transition: transform 0.2s, background 0.3s;
        }

        .social-links a:hover {
            background: #155083;
            transform: translateY(-2px);
        }

        /* Ícones via CSS */
        .social-links a::before {
            content: '';
            display: inline-block;
            width: 20px;
            height: 20px;
            background-size: contain;
        }

        .linkedin::before {
            background-image: url('data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij48cGF0aCBkPSJNMTkgMGgtMTRjLTIuNzYxIDAtNSAyLjIzOS01IDV2MTRjMCAyLjc2MSAyLjIzOSA1IDUgNWgxNGMyLjc2MiAwIDUtMi4yMzkgNS01di0xNGMwLTIuNzYxLTIuMjM4LTUtNS01em0tMTEgMTloLTN2LTExaDN2MTF6bS0xLjUtMTIuMjY4Yy0uOTY2IDAtMS43NS0uNzktMS43NS0xLjc2NHMuNzg0LTEuNzY0IDEuNzUtMS43NjQgMS43NS43OSAxLjc1IDEuNzY0LS43ODMgMS43NjQtMS43NSAxLjc2NHptMTMuNSAxMi4yNjhoLTN2LTUuNjA0YzAtMy4zNjgtNC0zLjExMy00IDB2NS42MDRoLTN2LTExaDN2MS43NjVjMS4zOTYtMi41ODYgNy0yLjc3NyA3IDIuNDc2djYuNzU5eiIvPjwvc3ZnPg==');
        }

        .instagram::before {
            background-image: url('data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij48cGF0aCBkPSJNMTIgMi4xNjNjMi45OTQgMCAzLjM1NS4wMTIgNC41NC4wNyAzLjY3Mi4xNjQgNS4wNSAyLjE5IDUuMjIgNS43MjYuMDU4IDEuMDEuMDcgMS4wMjguMDcgNC41NiAwIDMuNTMtLjAxMiAzLjU5My0uMDcgNC41Ni0uMTcgMy41MzYtMS41NDggNS41NjItNS4yMiA1LjcyNi0xLjE4NS4wNTgtMS41NDEuMDctNC41NDAuMDctMyAwLTMuMzU0LS4wMTItNC41NC0uMDctMy42NzItLjE2NC01LjA1LTIuMTktNS4yMi01LjcyNi0uMDU4LTEuMDEtLjA3LTEuMDI4LS4wNy00LjU2IDAtMy41MjguMDEyLTMuNTkuMDctNC41Ni4xNy0zLjUzNyAxLjU0OC01LjU2MiA1LjIyLTUuNzI2IDEuMTg2LS4wNTggMS44MzYtLjA3IDQuNTQtLjA3em0wIDEuNjI4Yy0zLjIwMyAwLTMuNDQzLjAxLTQuNTQyLjA2NS0yLjg2Ni4xMy0zLjg5MiAxLjA1OC00LjA2NiA0LjA2NS0uMDU1IDEuMTA4LS4wNjQgMS4zNDgtLjA2NCA0LjU0MiAwIDMuMTk0LjAwOSAzLjQzMy4wNjQgNC41NDEuMTc0IDMuMDE1IDEuMjA4IDMuOTM1IDQuMDY2IDQuMDY1IDEuMTAxLjA1NSAxLjMzOS4wNjQgNC41NDIuMDY0IDMuMjA0IDAgMy40NC0uMDA5IDQuNTQyLS4wNjQgMi44NjctLjEzIDMuODkyLTEuMDU4IDQuMDY1LTQuMDY1LjA1NS0xLjEwOC4wNjQtMS4zNDguMDY0LTQuNTQxIDAtMy4xOTQtLjAwOS0zLjQzMy0uMDY0LTQuNTQyLS4xNzQtMy4wMTUtMS4yMDgtMy45MzUtNC4wNjUtNC4wNjUtMS4xLS4wNTUtMS4zNC0uMDY1LTQuNTQyLS4wNjV6bTAgMy4wNjhjLTIuNzEgMC00LjkgMi4xOS00LjkgNC45IDAgMi43MSAyLjE5IDQuOSA0LjkgNC45IDIuNzEgMCA0LjktMi4xOSA0LjktNC45IDAtMi43MS0yLjE5LTQuOS00LjktNC45em0wIDguMDZjLTEuNzI1IDAtMy4xMy0xLjQwNS0zLjEzLTMuMTMgMC0xLjcyNSAxLjQwNS0zLjEzIDMuMTMtMy4xMyAxLjcyNSAwIDMuMTMgMS40MDUgMy4xMyAzLjEzIDAgMS43MjUtMS40MDUgMy4xMy0zLjEzIDMuMTN6bTUuMTM0LTkuMDRjMCAuNjM2LS41MTYgMS4xNS0xLjE1IDEuMTUtLjYzMyAwLTEuMTUtLjUxNC0xLjE1LTEuMTUgMC0uNjM0LjUxNy0xLjE1IDEuMTUtMS4xNS42MzQgMCAxLjE1LjUxNiAxLjE1IDEuMTV6bS0xLjQ0NyA1LjM3Yy0uNDAzLS4UzEzLjQyNyAxNiAxMiAxNnMtMy41NTMtMS42My00LjY4Ni00LjY4N2MtLjU1Ni0xLjYzLS42OTUtMy4zNDEtLjM3NS00LjMxM0M3LjM0yA2LjE4IDguODY4IDUgMTIgNWM0LjEzIDAgNSAxLjg5IDQuNjg4IDUuNjg4LS4yNDYgMi45MzgtMS44NzggNC4zMTItNC42ODggNC4zMTJzLTQuNDQyLTEuMzc1LTQuNTUzLTQuMTI1aDIuMDAxYy4xMDggMS42NjcgMS42MDggMy4xMjUgMy41NTIgMy4xMjUgMi4wMSAwIDMuNTUxLTEuNCAzLjU1MS0zLjU1aC0yLjV2LTEuNWg0LjV2Ni4wMDFoLTEuOTk5eiIvPjwvc3ZnPg==');
        }
    </style>
</head>
<body>
    <div class="card">
        <div class="profile-header">
            <h1>Jean Carlo Brudna dos Santos</h1>
            <h2>Assessor de Investimentos</h2>
        </div>

        <div class="contact-info">
            <p>📞 (55) 98471-2734</p>
            <p>📧 <a href="mailto:jean.brudna@reddereinvestimentos.com.br">jean.brudna@reddereinvestimentos.com.br</a></p>
            <p>🌐 <a href="https://reddereinvestimentos.com.br/" target="_blank">reddereinvestimentos.com.br</a></p>
        </div>

        <div class="social-links">
            <a href="https://www.linkedin.com/in/jean-carlo-brudna-dos-santos-a8706459/" target="_blank" class="linkedin">LinkedIn</a>
            <a href="https://www.instagram.com/jeancarlobds?igsh=bG83azV0bGJsZ21l" target="_blank" class="instagram">Instagram</a>
        </div>
    </div>
</body>
</html>
