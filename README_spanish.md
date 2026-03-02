# Preguntas Frecuentes

## 1. No aparece el cuadro de diálogo
Este mod requiere un programa backend adicional para ejecutarse. Descargue el programa backend localizado aquí: [https://github.com/szmania/Voices_of_the_Court/releases/latest](https://github.com/szmania/Voices_of_the_Court/releases/latest). El archivo .exe descargado se instalará automáticamente al abrirlo.

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

## Licencia y Atribución

### Información del Mod
- **Nombre del Mod**: Voices of the Court - Community Edition (VOTC-CE)
- **Licencia**: GNU General Public License v3.0 (GPLv3)
- **Versión de CK3 compatible**: 1.18 "Crane"

### Créditos y Atribución
Este proyecto es una obra derivada basada en VOTC / AliChat. Nos gustaría expresar nuestra profunda gratitud a los desarrolladores que mantuvieron este proyecto vivo y ampliaron los límites de la IA en Crusader Kings III:

**Creadores originales**: El equipo VOTC y los contribuyentes de la comunidad.

**Desarrollo continuo**: Un agradecimiento especial a la comunidad de desarrollo china, incluidos Lisiyuan233, zhaowendao2005 y otros que proporcionaron actualizaciones críticas y apoyo.

**Apoyo de la comunidad**: Gracias a Durond y MrAndroPC y a la comunidad en general por sus ideas y contexto histórico sobre el proyecto.

**Mantenedores de la Edición Comunitaria**: El equipo VOTC-CE y los contribuyentes.

### Información de licencia
Algunos de los materiales fuente originales de este mod se publicaron bajo la licencia Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0).

De acuerdo con la sección 4(b) de la licencia CC BY-SA 4.0, esta obra derivada se está licenciando bajo una licencia compatible con BY-SA: la GNU General Public License v3.0 (GPLv3).

- **Licencia original**: CC BY-SA 4.0
- **Licencia actual**: GPLv3

### Aviso GPLv3
Este programa es software libre: puede redistribuirlo y/o modificarlo bajo los términos de la GNU General Public License publicada por la Free Software Foundation, ya sea la versión 3 de la Licencia o (a su elección) cualquier versión posterior.

Este programa se distribuye con la esperanza de que sea útil, pero SIN NINGUNA GARANTÍA; incluso sin la garantía implícita de COMERCIABILIDAD o IDONEIDAD PARA UN PROPÓSITO PARTICULAR. Consulte la GNU General Public License para obtener más detalles.

Debería haber recibido una copia de la GNU General Public License junto con este programa. Si no, consulte <https://www.gnu.org/licenses/>.
