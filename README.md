<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Campanha Outubro Rosa</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9;
            color: #333;
        }
        header {
            background-color: #ff69b4; /* Rosa */
            color: white;
            padding: 20px;
            text-align: center;
        }
        main {
            padding: 20px;
        }
        img {
            max-width: 100%;
            height: auto;
            border-radius: 8px;
            margin-bottom: 20px;
        }
        .content, .prevention {
            margin-top: 20px;
            padding: 15px;
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        h2 {
            color: #ff69b4;
        }
        .footer {
            text-align: center;
            padding: 10px;
            background-color: #ff69b4;
            color: white;
            position: relative;
            bottom: 0;
            width: 100%;
        }
        .toggle {
            cursor: pointer;
            color: #007bff;
            text-decoration: underline;
        }
        .hidden {
            display: none;
        }
    </style>
</head>
<body>

<header>
    <h1>Outubro Rosa: Campanha de Conscientização sobre o Câncer de Mama</h1>
</header>

<main>
    <img src="https://i0.wp.com/oncoegenetica.com.br/wp-content/uploads/2020/09/cancer-de-mama.jpg" alt="Prevenção do Câncer de Mama">
    
    <div class="content">
        <h2>Importância do Autocuidado</h2>
        <p>
            O câncer de mama é um dos tipos de câncer mais comuns entre mulheres no Brasil. O Ministério da Saúde lançou uma campanha de autocuidado para conscientizar sobre a importância do diagnóstico precoce e da prevenção.
        </p>
        <p>
            A campanha, intitulada "Mulher: seu corpo, sua vida", visa estimular as mulheres a se conectarem com sua saúde, promovendo o autocuidado contínuo.
        </p>
        <p>
            Para mais informações, acesse a notícia completa: 
            <a href="https://www.gov.br/saude/pt-br/assuntos/noticias/2024/outubro/outubro-rosa-ministerio-da-saude-lanca-campanha-e-reforca-autocuidado" target="_blank">Campanha Outubro Rosa</a>.
        </p>
    </div>

    <div class="prevention">
        <h2>Prevenção do Câncer de Mama</h2>
        <p>
            Clique para ver dicas de prevenção!
        </p>
        <div class="toggle" onclick="togglePrevention()">Mostrar Dicas</div>
        <ul id="preventionList" class="hidden">
            <li>Realizar exames clínicos das mamas regularmente.</li>
            <li>Executar a mamografia conforme as orientações médicas.</li>
            <li>Manter uma alimentação saudável e equilibrada.</li>
            <li>Praticar atividades físicas regularmente.</li>
            <li>Evitar o consumo excessivo de álcool.</li>
            <li>Não fumar e evitar a exposição a substâncias cancerígenas.</li>
            <li>Amamentar, quando possível, pois isso pode reduzir o risco.</li>
        </ul>
        <p>
            Conhecer seu corpo e estar atenta a quaisquer mudanças é fundamental para a detecção precoce.
        </p>
    </div>
</main>

<footer class="footer">
    <p>&copy; 2024 Gustavo Alcântara</p>
</footer>

<script>
    function togglePrevention() {
        const list = document.getElementById('preventionList');
        list.classList.toggle('hidden');
        const toggleText = list.classList.contains('hidden') ? 'Mostrar Dicas' : 'Ocultar Dicas';
        document.querySelector('.toggle').innerText = toggleText;
    }
</script>

</body>
</html>
