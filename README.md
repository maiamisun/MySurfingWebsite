<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wyjazdy Surferskie</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f8f8f8;
            transition: background-color 0.3s ease-in-out;
        }
        header {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1em;
        }
        section {
            margin: 20px;
            padding: 20px;
            background-color: white;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
        }
        h2 {
            color: #333;
        }
        p {
            line-height: 1.6;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1em;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
        form {
            max-width: 400px;
            margin: 0 auto;
        }
        label {
            display: block;
            margin-bottom: 8px;
        }
        input, select, button {
            width: 100%;
            padding: 10px;
            margin-bottom: 16px;
            box-sizing: border-box;
        }
        button {
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            transition: background-color 0.3s ease-in-out;
        }
        button:hover {
            background-color: #45a049;
        }
        @media (max-width: 768px) {
            body {
                font-size: 14px;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Wyjazdy Surferskie</h1>
    </header>
    <section>
        <h2>Odkryj Nowe Fale</h2>
        <p>Zaplanuj swoją niesamowitą przygodę na desce. Znajdź najlepsze miejsca na surfowanie i doświadcz ekscytujących fal na całym świecie.</p>
    </section>
    <section>
        <h2>Najlepsze Destynacje</h2>
        <ul>
            <li><strong>Hawaje:</strong> Wyspy Hawajskie - raj dla surferów.</li>
            <li><strong>Bali:</strong> Piękne fale i kultura Indonezji.</li>
            <li><strong>Gold Coast:</strong> Złote wybrzeże Australii, świetne dla zaawansowanych surferów.</li>
        </ul>
    </section>
    <section>
        <h2>Atrakcje Dodatkowe</h2>
        <p>W naszych wyjazdach oferujemy nie tylko surfowanie, ale także różnorodne atrakcje, takie jak szkoły surfingu, relaks na plaży, i wiele innych.</p>
    </section>
    <section>
        <h2>Preferencje Wyjazdowe</h2>
        <form id="preferencesForm">
            <label for="destination">Preferowana Destynacja: </label>
            <input type="text" id="destination" name="destination" required>

            <label for="experience">Doświadczenie w Surfowaniu: </label>
            <select id="experience" name="experience" required>
                <option value="beginner">Początkujący</option>
                <option value="intermediate">Średniozaawansowany</option>
                <option value="advanced">Zaawansowany</option>
            </select>

            <button type="submit">Znajdź Idealny Wyjazd!</button>
        </form>
    </section>
    <footer>
        <p>&copy; 2024 Wyjazdy Surferskie. Wszelkie prawa zastrzeżone.</p>
    </footer>

    <script>
        document.getElementById("preferencesForm").addEventListener("submit", function(event) {
            event.preventDefault();
            const destination = document.getElementById("destination").value;
            const experience = document.getElementById("experience").value;
            alert(`Dziękujemy! Znajdziemy dla Ciebie idealny wyjazd do ${destination}. Twój poziom doświadczenia: ${experience}.`);
        });
    </script>
</body>
</html>
