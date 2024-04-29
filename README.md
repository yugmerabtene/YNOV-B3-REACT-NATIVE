### CHAPITRE-01 : Javascript Vanilla  
## TP-01 :  

**Titre:** Création d'une Calculatrice Simple en HTML et JavaScript

**Description:**
Dans ce TP, vous allez créer une calculatrice simple en utilisant HTML pour la structure et JavaScript pour la logique de calcul. Cette calculatrice permettra à l'utilisateur d'effectuer des opérations d'addition, de soustraction, de multiplication et de division sur deux nombres saisis.

**Objectifs:**
1. Mettre en pratique les connaissances en HTML pour créer l'interface utilisateur de la calculatrice.
2. Utiliser JavaScript pour implémenter la logique de calcul et la gestion des événements.
3. Permettre à l'utilisateur de saisir deux nombres et de choisir l'opération à effectuer.
4. Afficher le résultat de l'opération sur la page web.

**Tâches:**
1. Créer une page HTML avec les éléments nécessaires : deux champs de texte pour les nombres, des boutons pour les opérations et un élément pour afficher le résultat.
2. Utiliser JavaScript pour récupérer les valeurs saisies par l'utilisateur et effectuer les calculs en fonction de l'opération sélectionnée.
3. Afficher le résultat des calculs sur la page web.
4. Tester la calculatrice en saisissant différents nombres et en effectuant différentes opérations pour vérifier son bon fonctionnement.
5. Améliorer éventuellement la mise en forme et l'ergonomie de la calculatrice avec du CSS.

**Bonus:**
- Ajouter des fonctionnalités supplémentaires comme la possibilité de calculer des pourcentages, des racines carrées, etc.
- Permettre à l'utilisateur de saisir les nombres avec la souris en cliquant sur des boutons numériques plutôt que de les saisir manuellement.
- Ajouter des validations pour gérer les cas d'entrées non numériques ou les divisions par zéro.

**Ressources:**
- HTML pour la structure de la page web.
- JavaScript pour la logique de calcul et la gestion des événements.
- CSS pour améliorer la mise en forme de la calculatrice (facultatif).

**Corrigé :** 




<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculatrice</title>
</head>
<body>
    <h2>Calculatrice</h2>
    <input type="text" id="input1">
    <input type="text" id="input2">
    <button onclick="calculate('+')">+</button>
    <button onclick="calculate('-')">-</button>
    <button onclick="calculate('*')">*</button>
    <button onclick="calculate('/')">/</button>
    <p>Résultat : <span id="result"></span></p>

    <script>
        function calculate(operator) {
            let input1 = document.getElementById('input1').value;
            let input2 = document.getElementById('input2').value;
            let result;

            switch(operator) {
                case '+':
                    result = Number(input1) + Number(input2);
                    break;
                case '-':
                    result = Number(input1) - Number(input2);
                    break;
                case '*':
                    result = Number(input1) * Number(input2);
                    break;
                case '/':
                    result = Number(input1) / Number(input2);
                    break;
                default:
                    result = "Opérateur non valide";
            }

            document.getElementById('result').innerText = result;
        }
    </script>
</body>
</html>







# CHAPITRE-02 : REACT-NATIVE 





PROBLEME DEVICE MANAGER

https://www.journaldunet.fr/developpeur/developpement/1516329-comment-corriger-l-erreur-de-l-emulateur-android-the-emulator-process-for-avd-pixel-4-api-30-has-terminated/#:~:text=Une%20dernière%20solution%20pour%20résoudre,d%27Android%20va%20être%20désinstallé.
