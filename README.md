<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <link rel="stylesheet" type="text/css" href="formulario.css" media="screen">
        <title> Formulário </title>
        <style>
            *{
                margin: 0;
                padding: 0;
            }
            #titulo{
                font-family: sans-serif;
                color: #380B61;
                margin-left: 7%;
            }
            #subtitulo{
                font-family: sans-serif;
                color:#380B61;
                margin-left: 10%;
            }
            fieldset{
                border: 0;
            }
            body{
                background-color: #f0f0ff;
                font-family: sans-serif;
                font-size: 1em;
                color: #59429d;
                margin-left: 36%;
                justify-content: centerf;
            }
            input, select, textarea, button{
                border-radius: 5px;
            }
            .campo{
                margin-bottom: 1em;
            }
            .campo label{
                margin-bottom: 0.2em;
                color:#59429d;
                display: block;
            }
            fieldset.grupo .campo{
                float: left;
                margin-right: 1em;
            }
            .campo input[type="text"], .campo input[type="email"], .campo select, .campo textarea {
                padding: 0,2em;
                border: 1px solid #59429d;
                box-shadow: 2px 2px 2px rgba(0,0,0,0.2);
                display: block;
            }
            .campo select option{
                padding-right: 1em;
            }
            .campo input:focus, .campo select:focus, .campo textarea:focus {
                background: #e0e0f8;
            }
            .botao{
                font-size: 1.2em;
                background: #59429d;
                border: 0;
                margin-bottom: 1em;
                color:#ffffff;
                padding: 0.2em 0.6em;
                box-shadow: 2px 2px 2px rgba(0,0,0,0.2);
                text-shadow: 1px 1px 1px rgba(0,0,0,0.5);
                position: absolute;
                top: 90%;
                left: 50%;
                margin-right: -50%;
                transform: translate(-50%, -50%);
            }
            .botao:hover{
                background: #ccbbff;
                box-shadow: inset 2px 2px 2px rgba(0,0,0,0.2);
                text-shadow: none;
            }
            .botao, select{
            cursor: pointer;
            }
            #check{
            display: inline-block;
            }
        </style>
    </head>
    <body>
        <div class="campo">
            <h1 id="titulo"> Formulário Desmistificante</h1>
            <br>
        </div>
        <form>
            <fieldset class="grupo">
                <div class="campo">
                    <label for="nome"> <strong> Nome </strong> </label>
                    <input type="text" name="nome" id="nome" required>
                </div>
                <div class="campo">
                    <label for="sobrenome"> <strong> Sobrenome </strong> </label>
                    <input type="text" name="sobrenome" id="sobrenome" required>
                </div>
            </fieldset>
            <div class="campo">
                <label for="email"> <strong> Email </strong> </label>
                <input type="email" name="email" id="email" required>
            </div>
            <div class="campo">
                <label> <strong> Seu Comentário é Sobre: </strong> </label>
                <label> 
                    <input type="radio" name="comentario" value="Site em Geral" checked>Site em Geral
                </label>
                <label>
                    <input type="radio" name="comentario" value="Formulário">Formulário
                </label>
                <label>
                    <input type="radio" name="comentario" value="Recomendações">Recomendações
                </label>
            </div>
            <div class="campo">
                <label for="Comentário"> <strong> Seu Comentário é: </strong> </label>
                <select id="Comentário">
                    <option selected disabled value=""> Selecione </option>
                    <option> Construtivo </option>
                    <option> Neutro </option>
                    <option> Destrutivo </option>
                </select>
            </div>
            <fieldset class="grupo">
                <div id="check">
                    <label> <strong> Pois eu: </strong> </label>
                    <input type="checkbox" id="pois1" name="pois1" value="Achei Péssimo">
                    <label for="pois1"> Achei Péssimo </label>
                    <input type="checkbox" id="pois2" name="pois2" value="Achei Mal Acabado">
                    <label for="pois2"> Achei Mal Acabado </label>
                    <input type="checkbox" id="pois3" name="pois3" value="Achei Bem Acabado">
                    <label for="pois3"> Achei Bem Acabado </label>
                    <input type="checkbox" id="pois4" name="pois4" value="Achei Bom">
                    <label for="pois4"> Achei Bom </label>
                </div>
            </fieldset>
            <div class="campo">
                <br>
                <label> <strong> Fale Que Eu Te Escuto </strong> </labedl>
                <textarea row="6" style="width: 26em" id="falarescutar"></textarea>
            </div>
            <button class="botao" type="submit"> Enviar </button>
        </form>
    </body>
</html>
