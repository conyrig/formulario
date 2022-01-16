# Formulário sobre programação com HTML e CSS

<!DOCTYPE html>
<html lang="en">
<head>
    <!-- Metadados -->
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <!-- CSS -->
    <link rel="stylesheet" type="text/css" href="formulario.css" media="screen">
  
     <!-- Título da página (aparece na aba) -->
    <title>Registo</title>
</head>
<body>

    <!-- Cabeçalho com título e subtítulo (ambos com css de id "titulo") -->
    <div>
        <h1 id="titulo"> Questionário sobre programação </h1>
        <p id="subtitulo"> Complete o registo com as suas informações</p>
        <br>
    </div>
    
    <!-- Início do formulário -->
    <form>
        <fieldset class="grupo">
          <!-- Campo do nome com legenda "nome" e css de classe "campo" -->
            <div class="campo">
                <label for="nome"><strong>Nome</strong></label>
                <input type="text" name="nome" id="nome" required>
            </div>
           <!-- Campo do sobrenome com legenda "apelido" e css de classe "campo" -->
            <div class="campo">
                <label for="apelido"><strong>Apelido</strong></label>
                <input type="text" name="apelido" id="apelido" required>
            </div>
        </fieldset>

        <!-- Campo de email com-->
        <div class="campo">
            <label for="email"><strong>E-mail</strong></label>
            <input type="email" name="email" id="email" required>
        </div>

        <!-- Campo de desenvolvimento web com 3 opções de botões selecionáveis (radio button) e css de classe "campo" -->
        <div class="campo">
            <label> Qual o lado da aplicação que desenvolve? </label>
            <label>
                <input type="radio" name="devweb" value="frontend">Front-end
            </label>
            <label>
                <input type="radio" name="devweb" value="backend">Back-end
            </label>
            <label>
                <input type="radio" name="devweb" value="fullstack">Fullstack
            </label>
        </div>
        
       <!-- Campo de senioridade com 3 opções para escolha (select option) e css de classe "campo" -->
        <div class="campo">
            <label>SeniorIdade</label>
            <select id="SeniorIdade">
                <option selected disabled value="">Selecione</option>
                <option>Junior</option>
                <option>Pleno</option>
                <option>Senior</option>
            </select>
        </div>

        <!-- Campo de tecnologias para escolha de 1 ou mais opções para marcar (checkbox) e css de classe "campo" -->
        <fieldset class="grupo">
            <div id="check">
                <label> Selecione as linguagens que utiliza: </label><br><br>
                <input type="checkbox" id="tecnologia1" name="tecnologia1" value="HTML">
                <label for="tecnologia1">HTML</label>
                <input type="checkbox" id="tecnologia2" name="tecnologia2" value="CSS">
                <label for="tecnologia2">CSS</label>       
                <input type="checkbox" id="tecnologia3" name="tecnologia3" value="PHP">
                <label for="tecnologia3">PHP</label>
                <input type="checkbox" id="tecnologia4" name="tecnologia4" value="C">
                <label for="tecnologia4">C</label>
                <input type="checkbox" id="tecnologia5" name="tecnologia5" value="Python">
                <label for="tecnologia5">Python</label>
                <input type="checkbox" id="tecnologia6" name="tecnologia6" value="Java">
                <label for="tecnologia6">Java</label>
            </div>
        </fieldset>

       <!-- Caixa de texto -->
        <div class="campo">
            <br>
            <label> Conte um pouco da sua experiência: </label>
            <textarea row="6" style="width: 26em" id="experiencia" name="experiencia"></textarea>
        </div>

       <!-- Botão para enviar o formulário -->
        <button class="botao" type="submit">Concluído</button>

    </form>

</body>
</html>
