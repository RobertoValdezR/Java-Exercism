# java-exercism

Mis soluciones al [track de Java de Exercism](https://exercism.org/tracks/java/exercises).

Proyecto **Maven** con un paquete por ejercicio y sus tests en JUnit 5.

## Requisitos

| Qué | Cómo |
|---|---|
| JDK 21 (o 17+) | [Adoptium Temurin](https://adoptium.net/) — marca *"Set JAVA_HOME variable"* durante la instalación |
| VS Code | Extensión **Extension Pack for Java** (`vscjava.vscode-java-pack`) |

No hace falta instalar Maven aparte: la extensión de Java de VS Code trae su propio Maven embebido y descarga las dependencias sola.

## Estructura

```
java-exercism/
├── pom.xml                              <- dependencias (JUnit 5, AssertJ) y versión de Java
├── src/
│   ├── main/java/<ejercicio>/Clase.java      <- aquí escribes tu solución
│   └── test/java/<ejercicio>/ClaseTest.java  <- los tests (no se tocan)
└── .vscode/extensions.json
```

Cada ejercicio es un **paquete** (una carpeta con su `package` declarado arriba del archivo).
Añadir un ejercicio nuevo = crear su carpeta en `main` y en `test`.

## Cómo trabajar

1. Abre la carpeta `java-exercism` en VS Code (**File → Open Folder**, no abras el archivo suelto).
2. Espera a que la barra de estado termine de importar el proyecto Maven la primera vez.
3. Abre la clase del ejercicio en `src/main/java/...` y complétala.
4. Corre los tests:
   - Icono del matraz (**Testing**) en la barra lateral → ▶ para correr todo o un test suelto.
   - O haz clic en la flecha verde que aparece junto a cada `@Test`.
   - O desde la terminal: `mvn test` (si tienes Maven instalado).

## Ejercicios

| # | Ejercicio | Concepto | Estado |
|---|---|---|---|
| 1 | Lasagna | Basics: constantes, métodos, aritmética | 🔲 |
| 2 | Annalyn's Infiltration | Booleans | — |
| 3 | Cars, Assemble! | Numbers | — |
