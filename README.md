# Proyectos en C++

Aquí encontrarás una colección de mis proyectos desarrollados en C++. Cada uno de ellos refleja mis habilidades y exploraciones en este lenguaje. Espero que encuentres inspiración y recursos útiles para tus propios proyectos. ¡Disfruta explorando!

## Proyecto: Adivina el Número

**Descripción:**
"Adivina el Número" es un juego interactivo en el que el jugador debe adivinar un número aleatorio generado por la computadora dentro de un rango específico. A medida que el jugador intenta adivinar, se le informa si su intento fue correcto o no, y se le restan vidas por cada intento fallido.

**Características del juego:**
- **Niveles de dificultad:** El juego ofrece tres niveles de dificultad:
  - **Fácil:** Adivina un número del 0 al 9 (3 vidas).
  - **Intermedio:** Adivina un número del 0 al 99 (10 vidas).
  - **Imposible:** Adivina un número del 0 al 999 (30 vidas).
- **Sistema de música y efectos de sonido:** Música de fondo y efectos de sonido que enriquecen la experiencia de juego.
- **Interfaz amigable:** Menús claros y mensajes que guían al jugador.

### Cómo jugar
1. Inicia el juego y selecciona un nivel de dificultad.
2. Intenta adivinar el número ingresando tu respuesta.
3. Si aciertas, ¡felicidades! Se incrementará tu contador de victorias. Si fallas, perderás una vida.
4. El juego termina cuando se acaban tus vidas o logras adivinar el número.

### Ejemplo de código
Aquí hay un fragmento del código del juego:

```cpp
int GeN(int dificulty) {
    srand(static_cast<unsigned int>(time(0)));
    
    switch (dificulty) {
        case 1:
            NR = rand() % 10;
            Vidas = 3;
            DF = "Fácil";
            break;
        case 2:
            NR = rand() % 100;
            Vidas = 10;
            DF = "Intermedio";
            break;
        case 3:
            NR = rand() % 1000;
            Vidas = 30;
            DF = "Imposible";
            break;
        default:
            cout << "ERROR: Número de dificultad no está en el rango." << endl;
            cout << "Se pone en modo fácil.";
            Sleep(1000);
            NR = rand() % 10;
            Vidas = 3;
            break;
    }
    return NR;
}
```

### Requisitos
- C++11 o superior
- Sistema operativo Windows (para la reproducción de sonido)

### Instrucciones de instalación
1. Clona el repositorio en tu máquina local.
2. Asegúrate de tener un compilador de C++ instalado.
3. Compila y ejecuta el programa para comenzar a jugar.

### Contribuciones
Si deseas contribuir a este proyecto, no dudes en hacer un fork del repositorio y enviar un pull request. Aprecio cualquier mejora o sugerencia.

### Licencia
Este proyecto está bajo la licencia GPL.

---

¡Espero que disfrutes jugando "Adivina el Número" y explorando otros proyectos! Si tienes preguntas o comentarios, no dudes en contactarme.
