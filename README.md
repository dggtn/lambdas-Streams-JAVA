 <header>
      <h1>Lambdas y Streams en Java</h1>
  </header>

  <section>
      <h2>Descripción del Proyecto</h2>
      <p>Este repositorio contiene un proyecto para aprender y practicar el uso de <strong>Lambdas</strong> y <strong>Streams</strong> en Java. El objetivo del proyecto es familiarizarse con las herramientas modernas de Java que permiten escribir código más limpio, conciso y funcional utilizando la programación funcional.</p>
  </section>

  <section>
      <h2>Objetivos del Proyecto</h2>
      <ul>
          <li>Introducir el concepto de expresiones lambda en Java.</li>
          <li>Explorar la API de Streams para manejar colecciones de datos de manera más eficiente.</li>
          <li>Aplicar conceptos avanzados como filtros, mapeos y reducciones con Streams.</li>
          <li>Realizar estadísticas y cálculos sobre listas de datos utilizando Streams.</li>
      </ul>
  </section>

  <section>
      <h2>Tecnologías Utilizadas</h2>
      <ul>
          <li><strong>Java 8+</strong>: Utilización de las características más modernas del lenguaje, como lambdas y streams.</li>
          <li><strong>Streams API</strong>: Para manejar y procesar colecciones de datos de manera funcional.</li>
          <li><strong>Lambdas</strong>: Expresiones funcionales para simplificar el manejo de colecciones y operaciones sobre ellas.</li>
      </ul>
  </section>

  <section>
      <h2>Funcionalidades Implementadas</h2>
      <p>Este proyecto permite realizar varias operaciones usando lambdas y streams:</p>
      <ul>
          <li><strong>Operaciones con Streams:</strong> Filtrar, mapear, ordenar y reducir colecciones de datos.</li>
          <li><strong>Estadísticas sobre listas de datos:</strong> Calcular estadísticas como el total de evaluaciones o el promedio de calificaciones.</li>
          <li><strong>Uso de Lambdas:</strong> Creación de funciones anónimas para operar sobre colecciones.</li>
          <li><strong>Optimización de código:</strong> Uso de streams y lambdas para hacer el código más limpio y eficiente.</li>
      </ul>
  </section>

  <section>
      <h2>Instrucciones para Ejecutar el Proyecto</h2>
      <p>Para ejecutar este proyecto en tu máquina local, sigue los siguientes pasos:</p>
      <ol>
          <li><strong>Clona el repositorio:</strong>
              <pre>git clone https://github.com/dggtn9/lambdas-Streams-JAVA.git</pre>
          </li>
          <li><strong>Accede al directorio del proyecto:</strong>
              <pre>cd lambdas-Streams-JAVA</pre>
          </li>
          <li><strong>Compila y ejecuta el proyecto:</strong>
              <p>Si utilizas un IDE como Eclipse o IntelliJ IDEA, simplemente abre el proyecto y ejecútalo.</p>
              <p>Si prefieres usar la línea de comandos, asegúrate de tener Java 8 o superior instalado y ejecuta el siguiente comando:</p>
              <pre>javac Main.java</pre>
              <pre>java Main</pre>
          </li>
      </ol>
  </section>

  <section>
      <h2>Estructura del Proyecto</h2>
      <p>La estructura básica del proyecto es la siguiente:</p>
      <pre>
lambdas-Streams-JAVA/
│
├── src/
│   ├── Main.java               # Clase principal que contiene la lógica del proyecto.
│   └── Estadisticas.java       # Clase para calcular estadísticas de las colecciones.
│
└── README.html                 # Este archivo README en formato HTML.
      </pre>
  </section>

  <section>
      <h2>Ejemplo de Código</h2>
      <p>A continuación, se muestra un ejemplo básico del uso de lambdas y streams en Java:</p>
      <pre>
import java.util.*;
import java.util.stream.*;

public class Main {
  public static void main(String[] args) {
      List<Integer> evaluaciones = Arrays.asList(75, 85, 90, 55, 60, 95);

      // Calcular el total de evaluaciones usando Streams
      int totalEvaluaciones = evaluaciones.stream()
                                          .mapToInt(Integer::intValue)
                                          .sum();

      System.out.println("Total de evaluaciones: " + totalEvaluaciones);

      // Calcular el promedio de evaluaciones usando Streams
      double promedio = evaluaciones.stream()
                                    .mapToInt(Integer::intValue)
                                    .average()
                                    .orElse(0);

      System.out.println("Promedio de evaluaciones: " + promedio);
  }
}
      </pre>
      <p>En este ejemplo, se utiliza el método <code>stream()</code> para crear un flujo de datos y se aplican operaciones como <code>mapToInt()</code> y <code>average()</code> para calcular estadísticas sobre una lista de evaluaciones.</p>
  </section>

  <section>
      <h2>Contribuciones</h2>
      <p>Si deseas contribuir al proyecto, sigue estos pasos:</p>
      <ol>
          <li><strong>Haz un fork del repositorio:</strong> Esto te permitirá tener tu propia copia para hacer cambios.</li>
          <li><strong>Crea una nueva rama:</strong> Antes de realizar cualquier cambio, crea una nueva rama con un nombre descriptivo:
              <pre>git checkout -b feature/nueva-funcionalidad</pre>
          </li>
          <li><strong>Realiza tus cambios:</strong> Agrega nuevas funcionalidades, corrige errores o mejora el código.</li>
          <li><strong>Haz commit de tus cambios:</strong>
              <pre>git commit -m "Descripción de los cambios realizados"</pre>
          </li>
          <li><strong>Sube tus cambios:</strong>
              <pre>git push origin feature/nueva-funcionalidad</pre>
          </li>
          <li><strong>Abre un pull request:</strong> Después de subir tus cambios, abre un pull request para que podamos revisar tus modificaciones.</li>
      </ol>
  </section>

  <section>
      <h2>Licencia</h2>
      <p>Este proyecto está bajo la licencia <strong>MIT</strong>. Puedes ver los detalles en el archivo <code>LICENSE</code>.</p>
  </section>

  <section>
      <h2>Agradecimientos</h2>
      <p>Agradecemos a todos los colaboradores que contribuyan a este proyecto, y a los profesores que nos guiaron en el aprendizaje de Lambdas y Streams en Java.</p>
  </section>

</body>
</html>
