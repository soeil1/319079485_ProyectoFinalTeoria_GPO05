# 🏭 Proyecto 2 Final Computacion Grafica 
# Casa Entorno 3D Interactivo con Animación Jerárquica y por Keyframes en OpenGL

**Proyecto Final de Computación Gráfica – UNAM (FI)**
**Autor:** Oscar Cruz Soria [@soeil1](https://github.com/soeil1)
🕰️ **Fecha limite de entrega:25 Noviembre 2025
📜 **Versión:** `v1.0.0`

---
## 🧭 Descripción General
Es un entorno 3D interactivo desarrollado en **C++ y OpenGL**, que presenta una casa-robot caminante en un paisaje desolado estilo steampunk. 
Este proyecto combina el modelado 3D, la animación por código y la programación gráfica moderna para crear una escena interactiva.
---
## 🕹️ Controles

| Acción | Tecla |
|--------|-------|
| Movimiento | W / A / S / D |
| Rotar cámara | Mouse |
| Iniciar/Detener Animación de Patas | **P** |
| Iniciar/Detener Recorrido Automatico | **L** |
| Ocultar/Mostrar Pared (2do piso) | **F** |
| Salir del programa | **ESC** |
---

## 💡 Características Principales

### 🐾 Animación por Keyframes
- **Sistema `PataAnimada`:** Una clase dedicada que controla la animación de las 4 patas de la casa.
- **Carga desde Archivo:** Las secuencias de movimiento de cada pata se cargan independientemente desde archivos de texto (`pata1_anim.txt`, `pata2_anim.txt`, etc.).
- **Reproductor de Recorrido:** Un sistema `ReproductorCamara` que carga un recorrido cinematográfico pregrabado (`camera_anim.txt`) para mostrar la escena.

### ⚙️ Animación Jerárquica y Algorítmica
- **Dron Volador:** Un dron compuesto por 5 mallas separadas (cuerpo, hélice izq., hélice der., pata izq., pata der.).
- **Movimiento Compuesto:** El cuerpo sigue una trayectoria circular (`sin`/`cos`), se tambalea verticalmente, y las hélices y patas rotan y oscilan en relación a la transformación del cuerpo.

### 🔎 Interacción y Dinamismo
- **Cámara Libre:** Control total de la cámara en primera persona (movimiento con `WASD` y rotación con `Mouse`).
- **Interacción por Proximidad (Puerta):** La puerta principal de la casa detecta la distancia de la cámara y se abre automáticamente al acercarse.
- **Interacción por Proximidad (Dish):** La antena (plato) en el techo detecta la cámara y comienza a girar cuando está lo suficientemente cerca.
- **Visor de Interiores:** Se puede ocultar/mostrar la pared frontal del segundo piso (`F`) para ver el interior amueblado.

### 🌄 Renderizado y Entorno
- Motor gráfico basado en **OpenGL**.
- **Múltiples Modelos 3D (.obj)**, incluyendo la casa, la base, las patas, el dron y los muebles interiores.
- **Skybox 360°:** Un entorno de cielo cúbico para crear una atmósfera inmersiva.

---
### 🧰 Librerías Utilizadas
- GLEW
- GLFW
- GLM
- SOIL2 / stb_image
- Assimp
---

## 🔧 Compilación y Ejecución

1. **Clonar o descargar el repositorio:**
  
2. **Abrir el proyecto en Visual Studio:**
   * Haz doble clic en `Proyecto Final Computacion Grafica.sln`.

3. **Configurar la compilación:**
   * Selecciona la plataforma x86 en visual studio

4. Listo, pudes compilar 
---

## 🎩 Autor

| Nombre | GitHub |
|--------|--------|
| Oscar Cruz Soria 319079485 | [@soeil1](https://github.com/soeil1) |

---
