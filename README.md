<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout de Aplicativo Responsivo</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            color: #333;
            line-height: 1.6;
        }

        .container {
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }

        header {
            background: #6200ea;
            color: white;
            padding: 1rem;
            text-align: center;
        }

        nav {
            background: #3700b3;
            color: white;
            padding: 1rem;
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
        }

        nav ul li {
            margin: 0 1rem;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }

        main {
            flex: 1;
            padding: 1rem;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
            align-items: center;
        }

        .card {
            background: white;
            border: 1px solid #ddd;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            padding: 1rem;
            margin: 1rem;
            flex: 1 1 calc(33% - 2rem);
            max-width: calc(33% - 2rem);
            text-align: center;
        }

        .card h3 {
            margin-bottom: 1rem;
            color: #6200ea;
        }

        footer {
            background: #6200ea;
            color: white;
            text-align: center;
            padding: 1rem;
        }

        @media (max-width: 768px) {
            .card {
                flex: 1 1 calc(50% - 2rem);
                max-width: calc(50% - 2rem);
            }
        }

        @media (max-width: 480px) {
            nav ul {
                flex-direction: column;
            }

            .card {
                flex: 1 1 100%;
                max-width: 100%;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Layout de Aplicativo Responsivo</h1>
        </header>

        <nav>
            <ul>
                <li><a href="#">Início</a></li>
                <li><a href="#">Sobre</a></li>
                <li><a href="#">Serviços</a></li>
                <li><a href="#">Contato</a></li>
            </ul>
        </nav>

        <main>
            <div class="card">
                <h3>Funcionalidade 1</h3>
                <p>Detalhes sobre a funcionalidade 1.</p>
            </div>
            <div class="card">
                <h3>Funcionalidade 2</h3>
                <p>Detalhes sobre a funcionalidade 2.</p>
            </div>
            <div class="card">
                <h3>Funcionalidade 3</h3>
                <p>Detalhes sobre a funcionalidade 3.</p>
            </div>
        </main>

        <footer>
            <p>&copy; 2024 Todos os direitos reservados.</p>
        </footer>
    </div>
</body>
</html>
