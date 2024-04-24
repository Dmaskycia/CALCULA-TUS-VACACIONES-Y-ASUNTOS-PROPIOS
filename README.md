<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Calculadora de Días Libres</title>
</head>
<body>
    <h1>Calculadora de Días Libres por Meses Trabajados</h1>
    <label for="monthsWorked">Ingrese los meses trabajados:</label>
    <input type="number" id="monthsWorked" min="0" placeholder="Meses trabajados">
    <button onclick="calculateDaysOff()">Calcular Días Libres</button>
    <p>Días Libres: <span id="daysOff">0</span></p>

    <script>
        function calculateDaysOff() {
            let monthsWorked = document.getElementById('monthsWorked').value;
            let daysOff = 0;
            
            // Suponiendo que por cada mes trabajado, el empleado gana 2 días libres
            daysOff = monthsWorked * 2;

            document.getElementById('daysOff').innerText = daysOff;
        }
    </script>
</body>
</html>
