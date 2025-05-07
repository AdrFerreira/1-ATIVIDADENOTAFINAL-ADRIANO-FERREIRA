<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Formulário de Contato</title>
  <style>
  body {
   font-family: Arial;
   background-color: white;
   padding: 50px;
}
  .formulario {
   max-width: 500px;
   margin: auto;
   background-color: #fff;
   padding: 30px;
   border-radius: 8px;
}
  h2 {
  text-align: center;
  color: #FF0000;
}
  label {
  display: block;
  margin-top: 15px;
  font-weight: 500;
}
  input, textarea {
  width: 100%;
  padding: 10px;
  margin-top: 6px;
  border: 1px solid #ccc;
  border-radius: 4px;
}
  button {
  margin-top: 20px;
  width: 105%;
  padding: 12px;
  background-color: blue;
  color: white;
  font-weight: normal;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}
  button:hover {
  background-color: #696969;
}
  .message {
  margin-top: 15px;
  font-weight: bold;
  text-align: center;
}
</style>
<script>
  function validarEmail(email) {
  const partes = email.split('@');
  if (partes.length !== 2) return false;
   const [nome, dominio] = partes;
  if (nome.length === 0 || !dominio.includes('.')) return false;
   const dominioPartes = dominio.split('.');
  if (
    dominioPartes.length < 2 ||
    dominioPartes[0].length === 0 ||
    dominioPartes[1].length === 0
    ) {
  return false;
}
  return true;
}
  function validacaoFormularioFormulario() {
   const nome = document.getElementById("nome").value;
   const email = document.getElementById("email").value;
   const mensagem = document.getElementById("mensagem").value;
   const mensagemDiv = document.getElementById("mensagemDiv");
  if (!nome || !mensagem) {
   mensagemDiv.textContent = "Preencha todos os campos.";
   mensagemDiv.style.color = "red";
  return false;
}
  if (!validarEmail(email)) {
   mensagemDiv.textContent = "E-mail inválido.";
   mensagemDiv.style.color = "red";
  return false;
}
   mensagemDiv.textContent = "Formulário Pronto"
   mensagemDiv.style.color = "green";
  return false;
}
</script>
</head>

<body>
  <div class="formulario">
  <h2>FORMULÁRIO</h2>
  <form onsubmit="return validacaoFormulario()">
  <label for="nome">Nome completo:</label>
  <input type="text" id="nome" name="nome" placeholder="Seu nome" required>
  
  <label for="email">E-mail:</label>
  <input type="email" id="email" name="email" placeholder="Email" required>
  
  <label for="mensagem">Mensagem:</label>
  <textarea id="mensagem" name="mensagem" rows="5" placeholder="Digite sua mensagem" required></textarea>
  
  <button type="submit">Pronto!</button>
  <div class="message" id="mensagemDiv"></div>
  </form>
  </div>
</body>
</html>
