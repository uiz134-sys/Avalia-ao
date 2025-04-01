# Avalia-ao

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Avaliação de 5 Estrelas</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 50px;
        }
        .stars {
            display: flex;
            justify-content: center;
            gap: 10px;
            font-size: 30px;
            cursor: pointer;
        }
        .star {
            color: gray;
        }
        .star.selected {
            color: gold;
        }
    </style>
</head>
<body>
    <h1>Avalie nosso serviço</h1>
    <div class="stars" id="stars">
        <span class="star" data-value="1">★</span>
        <span class="star" data-value="2">★</span>
        <span class="star" data-value="3">★</span>
        <span class="star" data-value="4">★</span>
        <span class="star" data-value="5">★</span>
    </div>
    <p id="rating-text">Clique para avaliar</p>
    <textarea id="comentario" rows="4" cols="50" placeholder="Deixe um comentário..."></textarea><br>
    <button onclick="enviarAvaliacao()">Enviar Avaliação</button>
 
    <script>
        const stars = document.querySelectorAll('.star');
        let rating = 0;
        
        stars.forEach(star => {
            star.addEventListener('click', function() {
                rating = this.getAttribute('data-value');
                document.getElementById('rating-text').innerText = `Você avaliou com ${rating} estrelas`;
                stars.forEach(s => s.classList.remove('selected'));
               for (let i = 0; i < rating; i++) {
                    stars[i].classList.add('selected');
                }
            });
        });
        
        function enviarAvaliacao() {
            const comentario = document.getElementById('comentario').value;
            alert(`Avaliação enviada!\nEstrelas: ${rating}\nComentário: ${comentario}`);
        }
    </script>
</body>
</html>
