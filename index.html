<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Liga de Fútbol - Jornadas</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 20px;
      background-color: #f5f5f5;
    }

    h1, h2 {
      text-align: center;
      color: #2c3e50;
    }

    .container {
      display: flex;
      justify-content: space-between;
      gap: 20px;
    }

    .jornadas {
      flex: 2;
    }

    .jornada {
      background-color: #ffffff;
      padding: 15px;
      border-radius: 10px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      margin-bottom: 20px;
    }

    .jornada h3 {
      margin-top: 0;
      color: #2980b9;
    }

    label {
      display: block;
      margin: 10px 0;
    }

    select {
      margin-left: 10px;
      padding: 5px;
    }

    .clasificacion {
      flex: 1;
      background-color: #ffffff;
      padding: 15px;
      border-radius: 10px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      height: fit-content;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 10px;
    }

    th, td {
      border: 1px solid #ccc;
      padding: 6px;
      text-align: center;
    }

    .destacado-azul {
      background-color: #d0e8ff;
      font-weight: bold;
    }

    .destacado-verde {
      background-color: #d9fdd3;
    }
  </style>
</head>
<body>

  <h1>Calendario de Jornadas - Liga de Fútbol</h1>

  <div class="container">
    <div class="jornadas" id="partidos-container"></div>

    <div class="clasificacion">
      <h2>Clasificación</h2>
      <table>
        <thead>
          <tr>
            <th>Pos.</th>
            <th>Equipo</th>
            <th>Pts</th>
          </tr>
        </thead>
        <tbody id="tabla-cuerpo"></tbody>
      </table>
    </div>
  </div>

  <script>
    const puntosIniciales = {
      "La Unión Atl": 61,
      "Juventud Torremolinos": 59,
      "UCAM": 50,
      "Atlético Antoniano": 49,
      "Almeria B": 48,
      "Xerez CD": 48,
      "CD Estepona": 45,
      "Águilas FC": 44
    };

    const jornadas = [
      {
        nombre: "Jornada 31",
        partidos: [
          ["Linares Deportivo", "Águilas FC"],
          ["San Fernando CD", "UCAM"],
          ["Atlético Antoniano", "Juventud Torremolinos"],
          ["La Unión Atl", "Cádiz CF Mirandilla"],
          ["Almeria B", "CD Estepona"],
          ["Xerez CD", "Don Benito"]
        ]
      },
      {
        nombre: "Jornada 32",
        partidos: [
          ["Águilas FC", "Granada B"],
          ["Juventud Torremolinos", "Almeria B"],
          ["CD Estepona", "San Fernando CD"],
          ["Cádiz CF Mirandilla", "Atlético Antoniano"],
          ["Orihuela CF", "La Unión Atl"],
          ["UCAM", "Minera"],
          ["Villanovense", "Xerez CD"]
        ]
      },
      {
        nombre: "Jornada 33",
        partidos: [
          ["Águilas FC", "La Unión Atl"],
          ["Don Benito", "UCAM"],
          ["Deportiva Minera", "CD Estepona"],
          ["San Fernando CD", "Juventud Torremolinos"],
          ["Atlético Antoniano", "Orihuela CF"],
          ["Xerez Deportivo", "Xerez CD"]
        ]
      },
      {
        nombre: "Jornada 34",
        partidos: [
          ["Águilas FC", "Atlético Antoniano"],
          ["CD Estepona", "Don Benito"],
          ["Juventud Torremolinos", "Minera"],
          ["RB Linense", "La Unión Atl"],
          ["Xerez CD", "Linares Deportivo"],
          ["UCAM", "Xerez Deportivo"],
          ["Orihuela CF", "Almeria B"]
        ]
      }
    ];

    function crearJornadas() {
      const container = document.getElementById("partidos-container");

      jornadas.forEach((jornada, index) => {
        const div = document.createElement("div");
        div.className = "jornada";

        const h3 = document.createElement("h3");
        h3.textContent = jornada.nombre;
        div.appendChild(h3);

        jornada.partidos.forEach((partido, i) => {
          const label = document.createElement("label");
          label.textContent = `${partido[0]} vs ${partido[1]}`;

          const select = document.createElement("select");
          select.id = `partido-${index}-${i}`;

          const op0 = new Option("Seleccionar resultado", "");
          const op1 = new Option(`${partido[0]} gana`, partido[0]);
          const empate = new Option("Empate", "empate");
          const op2 = new Option(`${partido[1]} gana`, partido[1]);

          select.appendChild(op0);
          select.appendChild(op1);
          select.appendChild(empate);
          select.appendChild(op2);

          select.addEventListener("change", calcularTabla);

          label.appendChild(select);
          div.appendChild(label);
        });

        container.appendChild(div);
      });
    }

    function calcularTabla() {
      const puntos = { ...puntosIniciales };

      const selects = document.querySelectorAll("select");
      selects.forEach(select => {
        const valor = select.value;
        if (!valor) return; // No contar si no se ha seleccionado

        const label = select.parentElement.textContent.split(" vs ");
        const local = label[0].trim();
        const visitante = label[1].split(" gana")[0].trim();

        if (valor === "empate") {
          if (puntos[local] !== undefined) puntos[local] += 1;
          if (puntos[visitante] !== undefined) puntos[visitante] += 1;
        } else {
          if (puntos[valor] !== undefined) puntos[valor] += 3;
        }
      });

      const clasificacion = Object.entries(puntos).sort((a, b) => b[1] - a[1]);

      const cuerpo = document.getElementById("tabla-cuerpo");
      cuerpo.innerHTML = "";

      clasificacion.forEach(([equipo, pts], index) => {
        const fila = document.createElement("tr");

        if (index === 0) {
          fila.classList.add("destacado-azul");
        } else if (index >= 1 && index <= 4) {
          fila.classList.add("destacado-verde");
        }

        fila.innerHTML = `
          <td>${index + 1}</td>
          <td>${equipo}</td>
          <td>${pts}</td>
        `;
        cuerpo.appendChild(fila);
      });
    }

    crearJornadas();
    calcularTabla();
  </script>

</body>
</html>

