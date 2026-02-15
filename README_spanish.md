# Preguntas Frecuentes

## 1. No aparece el cuadro de diálogo
Este mod requiere un programa backend adicional para ejecutarse. Descargue el programa backend localizado aquí: [https://github.com/Lisiyuan233/Voices_of_the_Court1/releases/tag/betaZh](https://github.com/Lisiyuan233/Voices_of_the_Court1/releases/tag/betaZh). El archivo .exe descargado se instalará automáticamente al abrirlo.

## 2. Problemas de configuración de la API
Se recomienda utilizar la API oficial de DeepSeek. En el menú desplegable para la conexión del modelo de diálogo, seleccione la página `custom(openai-compatible)` para configurar:
- URL del servidor: `https://api.deepseek.com/beta`
- Clave API: Ingrese su propia clave API, que puede solicitar en [https://platform.deepseek.com](https://platform.deepseek.com).

OpenAI y OpenRouter también deberían ser compatibles.

## 3. No aparece el cuadro de diálogo incluso cuando el programa backend se está ejecutando después de la instalación
**Solución**: Debe utilizar el mod de localización.

Métodos de instalación (elija uno):
1. Después de extraer los archivos del mod de localización descargados, sobrescriba los archivos originales del mod en el directorio de Steam Workshop directamente.
2. Coloque la carpeta del mod extraída `voices_of_the_court_mod-1.2.1-beta` en la carpeta de mods del juego. Luego, use el Bloc de notas para crear un nuevo archivo llamado `voices_of_the_court_mod-1.2.1-beta.mod` en la carpeta `Documents\Paradox Interactive\Crusader Kings III\mod` con el siguiente contenido:
version="1.0"
tags={
"Gameplay"
}
name="Voices of the Court mcc"
supported_version="1.13.1"
path="C:/Users/ [Su nombre de usuario de PC aquí] / Documents/Paradox Interactive/Crusader Kings III/mod/voices_of_the_court_mod-1.2.1-beta"

Si el cuadro de diálogo aún no aparece después de instalar y activar el mod de localización, es posible que la ruta de la carpeta de usuario de CK3 esté configurada incorrectamente, o que el juego esté en modo Ironman. Este mod no funciona en modo Ironman.

## 4. Error "TypeError: Cannot read properties of undefined (reading 'playerID')" con texto rojo al abrir la ventana de chat
**Solución**: Cree una carpeta llamada `run` en `Documents\Paradox Interactive\Crusader Kings III`. Ingrese a esa carpeta y cree un archivo de texto llamado `votc.txt`.

## 5. No se leen los recuerdos recientes al hablar con los personajes
**Solución**:
1. Este es un pequeño error en el programa backend del autor original; descargar el backend localizado soluciona esto.
2. También puede deberse a los límites de tokens de memoria. Ajuste el tamaño de `max memory tokens` en la página de configuración del programa backend. Después de ajustar los tokens de memoria, también debe aumentar el `max new tokens`; es mejor si `max new tokens` es mayor que `max memory tokens`.

## 6. El script de generación de prompts se revierte después de reiniciar el programa backend
**Solución**:
Guárdelo como un archivo separado en la carpeta `custom`.
