# Se escucha 🎙️

Transcriptor de conversaciones en vivo, pensado para ayudar a mi abuela, que es sorda, a seguir conversaciones sin depender solo de la lectura de labios.

## Qué hace

- Transcribe lo que se habla en tiempo real
- Separa automáticamente a las distintas personas según el tono de su voz, mostrando cada una en un color distinto
- Detecta cambios de tono **mientras se está hablando**, sin esperar a una pausa larga, para no juntar en un solo bloque lo que dicen varias personas en una conversación rápida
- Compara cada frase nueva contra la media de las últimas frases de esa persona (no solo la última), para no confundirla con otra si varía un poco el tono
- Al terminar la conversación, permite ponerle un nombre real a cada persona detectada
- Recuerda las voces guardadas entre sesiones, para reconocer a la misma persona en conversaciones futuras sin tener que volver a nombrarla
- Modo oscuro, con detección automática de la preferencia del sistema y memoria de la elección
- Auto-scroll de toda la página a medida que llega texto nuevo

## Cómo usarlo

Abre la web publicada en Safari (funciona mejor en iPhone), dale permiso de micrófono, y pulsa "Empezar a escuchar". Se puede añadir a la pantalla de inicio desde el botón de compartir de Safari para que funcione como una app.

## Estado del proyecto

Prototipo en desarrollo activo, probado ya en conversaciones reales. Limitación conocida: el corte por cambio de tono obliga a reiniciar el motor de reconocimiento del navegador, lo que a veces pierde alguna palabra suelta justo en el punto de corte. Pendiente de afinar umbrales con más pruebas. Explorando también cómo extenderlo a videollamadas y a conversaciones de grupo grandes.
