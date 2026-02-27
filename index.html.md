<!DOCTYPE html>  
<html lang="fr">  
<head>  
<meta charset="UTF-8">  
<meta name="viewport" content="width=device-width, initial-scale=1.0">  
<title>Joyeux Anniversaire Nadi</title>  
  
<style>  
body{  
    margin:0;  
    padding:0;  
    font-family: Arial, sans-serif;  
    background-color: black;  
    color: white;  
    text-align: center;  
}  
  
.page{  
    display: none;  
    padding: 40px;  
    min-height: 100vh;  
}  
  
.active{  
    display: block;  
}  
  
img{  
    width: 250px;  
    height: 250px;  
    object-fit: cover;  
    border-radius: 50%;  
    border: 4px solid white;  
    margin-top: 20px;  
}  
  
.heart{  
    font-size: 60px;  
    color: red;  
}  
  
button{  
    margin-top: 30px;  
    padding: 10px 20px;  
    background: white;  
    color: black;  
    border: none;  
    cursor: pointer;  
    font-weight: bold;  
}  
  
button:hover{  
    background: gray;  
}  
</style>  
</head>  
  
<body>  
  
<!-- PAGE 1 -->  
<div class="page active" id="page1">  
    <div class="heart">❤️</div>  
    <h1>JOYEUX ANNIVERSAIRE NADI</h1>  
    <img src="nadi.jpg" alt="Photo de Nadi">  
    <br>  
    <button onclick="nextPage(2)">Suivant ➜</button>  
</div>  
  
<!-- PAGE 2 -->  
<div class="page" id="page2">  
    <h1>✨ Tous mes vœux pour toi ✨</h1>  
    <p>  
        Que cette nouvelle année de ta vie soit remplie de bonheur,  
        de réussite, de paix et d'amour.  
        <br><br>  
        Que tous tes rêves deviennent réalité.  
        Que tu continues d’illuminer le monde par ta beauté,  
        ton sourire et ton énergie.  
        <br><br>  
        Tu mérites le meilleur, aujourd’hui et toujours.  
    </p>  
    <button onclick="nextPage(1)">⬅ Retour</button>  
    <button onclick="nextPage(3)">Suivant ➜</button>  
</div>  
  
<!-- PAGE 3 -->  
<div class="page" id="page3">  
    <h1>💌 Messages de nous tous 💌</h1>  
    <p>  
        De la part de toutes nos connaissances communes,  
        nous te souhaitons une année exceptionnelle.  
        <br><br>  
        Que la santé, la réussite et la joie  
        t’accompagnent chaque jour.  
        <br><br>  
        Continue d’être cette personne incroyable  
        que nous avons eu le plaisir de connaître en 2025.  
    </p>  
    <button onclick="nextPage(2)">⬅ Retour</button>  
    <button onclick="nextPage(4)">Suivant ➜</button>  
</div>  
  
<!-- PAGE 4 -->  
<div class="page" id="page4">  
    <h1>🖤 Un message spécial 🖤</h1>  
    <p>  
        Nadi, ce petit site a été créé spécialement pour toi.  
        <br><br>  
        Depuis notre rencontre en 2025,  
        j’ai eu le plaisir de découvrir une personne  
        belle, élégante et unique.  
        <br><br>  
        Aujourd’hui, je voulais marquer ton anniversaire  
        d’une manière différente,  
        quelque chose qui reste,  
        quelque chose qui montre que ce jour compte.  
        <br><br>  
        Ce site est une trace,  
        un souvenir,  
        un petit geste pour te rappeler  
        que tu es spéciale.  
        <br><br>  
        Joyeux anniversaire encore une fois 🖤  
    </p>  
    <button onclick="nextPage(3)">⬅ Retour</button>  
</div>  
  
<script>  
function nextPage(pageNumber){  
    let pages = document.querySelectorAll(".page");  
    pages.forEach(page => page.classList.remove("active"));  
    document.getElementById("page" + pageNumber).classList.add("active");  
}  
</script>  
  
</body>  
</html>  
