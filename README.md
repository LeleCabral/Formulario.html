# Formulario.html
Cadastro de DEVs. Projeto HTML e CSS.

<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" type="text/css" href="formulario.css" media="screen">
    <title>cadastro de DEVs</title>
</head>
<body>
    <div>
        <h1 id="titulo">Cadastro de DEVs</h1>
        <p id="subtitulo">Complete suas informações</p>
    </div>
<form>
    <fieldset class="grupo"> 
        <div>
            <label for="nome"><strong>Nome</strong></label>
            <input type="text" name="nome" id="nome" required>
        </div>
        <div class="campo">
            <label for="sobrenome"><strong>Sobrenome</strong></label>
            <input type="text" name="sobrenome" id="sobrenome" required>
        </div>
    </fieldset>

    <div class="campo">
        <label for="email"><strong>Email</strong></label>
        <input type="email" name="email" id="email" required>
    </div>

    <div class="campo">
        <label><strong>Em qual aplicação você desenvolve?</strong></label>
        <label>
            <input type="radio" name="devweb" volue="frontend" checked>Front-end
        </label>
        <label>
            <input type="radio" name="devweb" value="backend">Back-end
        </label>
        <label>
            <input type="radio" name="devweb" value="fullstack">Fullstack
        </label>
    </div>

    <div>
        <label><strong>Senioridade</strong></label>
        <select id="senioridade">
            <option selected disabled value="">Selecione</option>
            <option>Junior</option>
            <option>Pleno</option>
            <option>Senior</option>
</select>
    </div>

<fieldset class="grupo"   >
    <div id="checkbox"></div>
        <label><strong>Selecione as tecnologias que você utiliza</strong></label>
        <input type="checkbox" id="tecnologia1" name="tecnologia1" value="HTML">
        <label for="tecnologia1">HTML</label>
        <input type="checkbox" id="tecnologia2" name="tecnologia2" value="css">
        <label for="tecnologia2">CSS</label>
        <input type="checkbox" id="tecnologia3" name="tecnologia3" value="Javascript">
        <label for="tecnologia3">Javascript</label>
        <input type="checkbox" id="tecnologia4" name="tecnologia4" value="PYthon">
        <label for="tecnologia4">PYthon</label>
        <input type="checkbox" id="tecnologia5" name="tecnologia5" value="Java">
        <label for="tecnologia5">Java</label>
        <input type="checkbox" id="tecnologia6" name="tecnologia6" value="C#">
        <label for="tecnologia6">C#</label>
    </div>
</fieldset>

<div>
    <label><strong>Fale um pouco sobre você, suas experiências e habilidades</strong></label>
    <textarea row="6" style="width: 26em" id="experiencia"></textarea>
</div>

<button class="button" type="submit">Enviar</button> 
</form>
</body>
</html>    


*{
    margin: 0;
    padding: 0;
}

#titulo{
    font-family: sans-serif;
    color: #640e60;
    margin-left: 7%;
}

#subtitulo{
    font-family: sans-serif;
    color: #640e60;
    margin-left: 10%;
}

#check {
    display: inline-block;
}

fieldset{
    border:0;
}

body{
    background-color: #F0F8FF;
    font-family: sans-serif;
    font-size: 1em;
    color: #852c76; 
    margin-left: 36%;
    margin-top: 2%;
    justify-content: center;
}

input, select, textarea, button{
    font-family: sans-serif;
    font-size: 1em;
    color:#59429d;
    border-radius: 5px;
}

.grupo:before, .grupo::after{
    display: table;
}

.grupo:after {
    clear: both;
}

.campo {
    margin-bottom: 1em;
}

.campo label{
    margin-bottom: 0.2em;
    color: #852c76;
    display: bloco;
}

fieldset.grupo .campo{
    float: left;
    margin-right: 1em;
}

.campo input[type="text"], .campo input[type="email"], .campo select, .campo textarea {
    padding: 0.2em;
    border: 1px solid #852c76;
    box-shadow: 2px 2px 2px rgba(0,0,0,0.2);
    display: block;
}

.campo select option{
    padding-right: 1em;
}

.campo input:focus, .campo select:focus, .campo textarea:focus {
    background: #E0E0F8;
}

.botao {
font-size: 1.2em;
background: #7a0e71;
border: 0;
margin-bottom: 1em;
color: #d12ebb;
padding: 0.2em 0.6em;
box-shadow: 2px 2px 2px rgba(0,0,0,0.2);
text-shadow: 1px 1px 1px rgba(0,0,0,0.5);
position: absolute;
top: 90%;
left: 50%;
margin-right: -50%;
transform: translate(-50%, -50%);
}
 .botao:hover {
    background: #ccbbff;
    box-shadow:inset 2px 2px 2px rgba(0,0,0,0.2);
    text-shadow:none;
 }

 .botao, select {
cursor: pointer;
 }


