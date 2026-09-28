# ATENA
Quizz de référence du label ATéNA
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quiz : Produits de Nouvelle-Aquitaine</title>
    <style>
        /* (Gardez le CSS précédent) */
    </style>
</head>
<body>
    <div class="container">
        <h1>Quiz : Produits alimentaires de Nouvelle-Aquitaine</h1>
        <p class="quiz-description">
            Testez vos connaissances sur les produits emblématiques de notre région !
        </p>
        <div id="timer" style="text-align: center; font-size: 1.2em; margin-bottom: 20px;">5:00</div>
        <div class="quiz-progress">
            <span>Question <span id="current-question">1</span> sur <span id="total-questions">1</span></span>
            <span>Score : <span id="score">0</span></span>
        </div>
        <div id="quiz-questions"></div>
        <div class="navigation">
            <button id="prev-btn" class="btn-secondary" disabled>Précédent</button>
            <button id="next-btn" class="btn-primary">Suivant</button>
        </div>
        <div class="results" id="results">
            <h2>Félicitations !</h2>
            <p class="feedback" id="feedback"></p>
            <p class="score">Votre score : <span id="final-score">0</span> / <span id="total-questions-result">1</span></p>
            <button id="restart-btn" class="btn-primary restart-btn">Recommencer</button>
        </div>
    </div>
    <script>
        const questions = [
            {
                question: "Quel fromage de chèvre AOP est produit en Nouvelle-Aquitaine et doit son nom à une déformation du mot arabe *chebli* ?",
                options: ["Rocamadour", "Chabichou du Poitou", "Crottin de Chavignol", "Cheblinon cendré"],
                correctAnswer: 1,
                image: "https://upload.wikimedia.org/wikipedia/commons/thumb/5/5a/Chabichou_du_Poitou.jpg/320px-Chabichou_du_Poitou.jpg",
                explanation: "Le Chabichou du Poitou est un fromage de chèvre AOP dont le nom vient du mot arabe *chebli* (chèvre), hérité de la bataille de Poitiers en 732."
            },
            {
                question: "Laquelle de ces huîtres est une spécialité de la région Arcachon-Cap Ferret ?",
                options: ["Huître plate du banc", "Huître creuse du Grand Banc", "Huître verte du banc de sable", "Huître perlière du lagon"],
                correctAnswer: 1,
                image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/Hu%C3%AEtre_creuse.jpg/320px-Hu%C3%AEtre_creuse.jpg",
                explanation: "L’huître creuse du Grand Banc est une spécialité de la région Arcachon-Cap Ferret, élevée dans le bassin d’Arcachon."
            },
            {
                question: "Quel vin rouge de Bordeaux bénéficiant d’une AOC est issu majoritairement du cépage Merlot ?",
                options: ["Sauternes", "Saint-Émilion", "Médoc", "Jurançon"],
                correctAnswer: 1,
                image: "https://upload.wikimedia.org/wikipedia/commons/thumb/7/7a/Saint-%C3%89milion_vineyard.jpg/320px-Saint-%C3%89milion_vineyard.jpg",
                explanation: "Le Saint-Émilion est un vin rouge de Bordeaux AOC, principalement issu du cépage Merlot."
            },
            {
                question: "Quelle est la spécialité sucrée à base d’un fruit de la région d’Agen ?",
                options: ["Tarte aux pommes", "Pruneau farci au foie gras", "Clafoutis", "Financiers"],
                correctAnswer: 1,
                image: "https://upload.wikimedia.org/wikipedia/commons/thumb/8/8a/Pruneaux_farcis.jpg/320px-Pruneaux_farcis.jpg",
                explanation: "Le pruneau farci au foie gras est une spécialité sucrée-salée typique d’Agen, associant le pruneau local et le foie gras du Sud-Ouest."
            },
            {
                question: "Lequel de ces produits est une AOC de la Charente ?",
                options: ["Cognac", "Armagnac", "Pineau des Charentes", "Floc de Gascogne"],
                correctAnswer: 0,
                image: "https://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Cognac_bottle.jpg/320px-Cognac_bottle.jpg",
                explanation: "Le Cognac est une AOC de la Charente, reconnue depuis 1936. C’est un spiritueux obtenu par distillation de vin blanc."
            }
            // Ajoutez vos 15 autres questions ici
        ];

        // (Gardez le reste du JavaScript précédent, y compris le chronomètre)
    </script>
</body>
</html>
