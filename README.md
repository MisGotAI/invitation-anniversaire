# invitation-anniversaire
birth
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Invitation d'Anniversaire</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f9f9f9;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
        }
        .invitation {
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            padding: 20px;
            text-align: center;
            max-width: 600px;
            width: 100%;
        }
        .invitation h1 {
            color: #333;
        }
        .invitation p {
            color: #666;
            margin: 20px 0;
        }
        .photos img {
            max-width: 100%;
            height: auto;
            border-radius: 5px;
            margin-bottom: 10px;
        }
        .rsvp {
            margin-top: 20px;
        }
        .rsvp label {
            display: block;
            margin-bottom: 10px;
        }
        .rsvp input[type="radio"] {
            margin-right: 5px;
        }
        .rsvp button {
            padding: 10px 20px;
            background-color: #007BFF;
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .rsvp button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="invitation">
        <h1>Invitation d'Anniversaire</h1>
        <p>Tu es invité(e) à mon anniversaire le 23 juin 2000 ! Rejoins-moi pour une journée de célébration et de plaisir.</p>
        <div class="photos">
            <img src="photo1.jpg" alt="Photo 1">
            <img src="photo2.jpg" alt="Photo 2">
        </div>
        <div class="rsvp">
            <label>Veuillez confirmer votre présence :</label>
            <label><input type="radio" name="rsvp" value="oui"> Je serai présent(e)</label>
            <label><input type="radio" name="rsvp" value="non"> Je ne pourrai pas venir</label>
            <button onclick="confirmRSVP()">Confirmer</button>
        </div>
    </div>

    <script>
        function confirmRSVP() {
            const rsvp = document.querySelector('input[name="rsvp"]:checked');
            if (rsvp) {
                alert(`Vous avez confirmé : ${rsvp.value === 'oui' ? 'présent(e)' : 'absent(e)'} !`);
            } else {
                alert('Veuillez sélectionner une option.');
            }
        }
    </script>
</body>
</html>
