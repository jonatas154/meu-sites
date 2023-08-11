<!DOCTYPE html>

 

<html>

 

<head>

 

<style>

 

  body {

 

    display: flex;

 

    justify-content: center;

 

    align-items: center;

 

    height: 100vh;

 

    margin: 0;

 

    background-color: #f0f0f0;

 

    font-family: Arial, sans-serif;

 

  }

 

 

 

  #content {

 

    text-align: center;

 

  }

 

 

 

  #question {

 

    font-size: 24px;

 

    margin-bottom: 20px;

 

  }

 

 

 

  #emojis {

 

    font-size: 40px;

 

  }

 

 

 

  .button {

 

    border: none;

 

    color: white;

 

    padding: 15px 32px;

 

    text-align: center;

 

    text-decoration: none;

 

    display: inline-block;

 

    font-size: 16px;

 

    margin: auto;

 

    background-color: #4d82ad;

 

    cursor: pointer;

 

  }

 

 

 

  #yesButton {

 

    background-color: #53a653;

 

    margin-right: 20px;

 

  }

 

 

 

  #noButton {

    position: absolute;

    background-color: #e04f5f;

  }

 

</style>

 

</head>

 

<body>

 

 

 

<div id="content">

 

  <div id="question">

 

    Você quer sair hoje a noite?

 

  </div>

 

  <div id="emojis">

 

    😂🤣😆😅😄😃

 

  </div>

 

  <button id="yesButton" class="button" onclick="showAgreement()">Não</button>

 

  <button id="noButton"class="button" onmouseover="moveButton(this)">Sim</button>

 

</div>

 

 

 

<script>

 

  function moveButton(x) {

 

    const marginX = Math.floor(Math.random() * 400);

 

    const marginY = Math.floor(Math.random() * 200);

 

 

 

    x.style.margin = marginY.toString() + 'px ' + marginX.toString() + 'px';

 

  }

 

 

 

  function showAgreement() {

 

    const contentDiv = document.getElementById('content');

 

    const yesButton = document.getElementById('yesButton');

 

 

 

    contentDiv.innerHTML = `

 

      <div id="question">

 

        Eu concordo com você

 

      </div>

 

      <div id="emojis">

 

        🙌😄👍

 

      </div>

 

    `;

 

    contentDiv.style.textAlign = 'center';

 

    yesButton.style.display = 'none';

 

  }

 

</script>

 

</body>

 

</html>
