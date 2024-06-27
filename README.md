<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Checklist Veicular</title>
  <style>
    /* Estilos opcionais para melhorar a aparência */
    body {
      font-family: Arial, sans-serif;
      max-width: 600px;
      margin: 0 auto;
      padding: 20px;
    }
    label {
      display: block;
      margin-bottom: 5px;
    }
    input, textarea {
      width: 100%;
      padding: 8px;
      margin-bottom: 10px;
      border: 1px solid #ccc;
      border-radius: 4px;
      box-sizing: border-box;
    }
    button {
      background-color: #4CAF50;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 4px;
      cursor: pointer;
    }
    button:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>
  <h2>Checklist Veicular - Auditoria de Entrada e Saída</h2>
  <form action="/submit" method="post" enctype="multipart/form-data">
    <label for="dono">Dono:</label>
    <input type="text" id="dono" name="dono" required>

    <label for="ano">Ano:</label>
    <input type="text" id="ano" name="ano" required>

    <label for="cor">Cor:</label>
    <input type="text" id="cor" name="cor" required>

    <label for="chassi">Chassi:</label>
    <input type="text" id="chassi" name="chassi" required>

    <label for="renavam">Renavam:</label>
    <input type="text" id="renavam" name="renavam" required>

    <label for="acessorios">Acessórios:</label>
    <textarea id="acessorios" name="acessorios" rows="3" required></textarea>

    <label for="motor">Motor:</label>
    <input type="text" id="motor" name="motor" required>

    <label for="observacao">Observação:</label>
    <textarea id="observacao" name="observacao" rows="3"></textarea>

    <label for="fotos">Fotos do Veículo (até 30 fotos):</label>
    <input type="file" id="fotos" name="fotos[]" accept="image/*" multiple required>

    <button type="submit">Enviar Auditoria</button>
  </form>
</body>
</html>
