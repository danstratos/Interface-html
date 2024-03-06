<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gestión de Planificaciones Académicas</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        .container {
            max-width: 800px;
            margin: 50px auto;
            padding: 20px;
            background-color: #fff;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h2 {
            text-align: center;
        }
        form {
            margin-bottom: 20px;
        }
        label {
            margin-bottom: 10px;
        }
        input[type="text"], input[type="submit"] {
            padding: 10px;
            margin-bottom: 20px;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 16px;
        }
        input[type="submit"] {
            background-color: #007bff;
            color: #fff;
            cursor: pointer;
        }
        input[type="submit"]:hover {
            background-color: #0056b3;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }
        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }
        th {
            background-color: #f2f2f2;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Ingresar Nuevo Profesor</h2>
        <form action="profesores.php" method="POST">
            <label for="nombre">Nombre:</label>
            <input type="text" id="nombre" name="nombre" required>
            <label for="email">Email:</label>
            <input type="text" id="email" name="email" required>
            <input type="submit" value="Guardar Profesor">
        </form>

        <h2>Ingresar Nueva Materia</h2>
        <form action="materias.php" method="POST">
            <label for="nombre_materia">Nombre de la Materia:</label>
            <input type="text" id="nombre_materia" name="nombre_materia" required>
            <input type="submit" value="Guardar Materia">
        </form>

        <h2>Ingresar Nuevo Evento</h2>
        <form action="eventos.php" method="POST">
            <label for="nombre_evento">Nombre del Evento:</label>
            <input type="text" id="nombre_evento" name="nombre_evento" required>
            <label for="tipo_evento">Tipo de Evento:</label>
            <input type="text" id="tipo_evento" name="tipo_evento" required>
            <input type="submit" value="Guardar Evento">
        </form>

        <h2>Lista de Profesores y Materias Asociadas</h2>
        <table>
            <tr>
                <th>Profesor</th>
                <th>Materias Asociadas</th>
            </tr>
            <tr>
                <td>Profesor 1</td>
                <td>Materia 1, Materia 2</td>
            </tr>
            <tr>
                <td>Profesor 2</td>
                <td>Materia 3, Materia 4</td>
            </tr>
            <!-- Puedes generar esta tabla dinámicamente desde tu backend -->
        </table>
    </div>
</body>
</html>


