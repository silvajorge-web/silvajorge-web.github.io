# silvajorge-web.github.io
El objetivo del proyecto es proporcionar una herramienta interactiva que permite a los usuarios calcular su impacto ambiental (específicamente su Huella de Carbono) basándose en su consumo de energía y uso de transporte.
<!DOCTYPE html>
<html lang ="es">
<!-- 
   Proyecto: Calculadora de Huella Ambiental
   Realizado dentro del proyecto PAE del CBTis No.1
   Programadores: Ma. Eugenia Acuña - Jorge Dávalos Silva - Adal Francisco Castro Leos - Diana Estefania Ibarra
   Fecha: Agosto 2025
-->
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">               
<title>Huella Ambiental</title>
<link rel="stylesheet" href="estilos.css">
</head>
<body>
   <header>
    <h1>Huella Ambiental</h1>
   </header>
   <main>
  <section id="calculadora-contenedor">
    <h2>Huella Ambiental </h2>

    <!-- Pestañas -->
    <div class="tabs">
      <button class="tablink active" onclick="openTab(event, 'tab1')">Calculadora de Huella de Carbono</button>
      <button class="tablink" onclick="openTab(event, 'tab2')">Equivalencias</button>
    </div>

    <!-- Contenido pestaña 1 -->
    <div id="tab1" class="tab-content active">
      <h3>Calculadora de Huella de Carbono</h3>
      <form>
        <label for="energia">Consumo de energía (kWh):</label>
        <input type="number" id="energia" name="energia">
        <br>
        <label for="transporte">Distancia en transporte público (km):</label>
        <input type="number" id="transporte" name="transporte">

        <button type="submit" id="calcular">Calcular</button>
      </form>

      <p id="resultado"></p>
    </div>

    <!-- Contenido pestaña 2 -->
    <div id="tab2" class="tab-content">
      <h3>Calcula tus equivalencias</h3>
      <label for="kWhInput">Introduce tu consumo en kWh:</label>
      <input type="number" id="kWhInput" placeholder="Ejemplo: 250">
      <button id="btnCalcularEquivalencias">Calcular</button>
      <div id="resultadoEquivalencias"></div>
    </div>
  </section>
  </main>

  <script src="script.js"></script>
</body>
</html>
