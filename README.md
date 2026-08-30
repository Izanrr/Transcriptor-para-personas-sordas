# Se escucha 🎙️

Transcriptor de conversaciones en vivo, pensado para ayudar a mi abuela, que es sorda, a seguir conversaciones sin depender solo de la lectura de labios.

## Qué hace

- Transcribe lo que se habla en tiempo real
- Separa a las distintas personas combinando varias señales: pausas cortas detectadas por un VAD propio (energía de audio, ~150ms), y una huella de voz de tres rasgos (tono, timbre/brillo espectral, proporción graves-medios) — no solo el tono
- Solo corta el texto cuando hay indicio real de cambio de hablante, con un margen de confianza, priorizando no perder palabras sobre la precisión del corte
- Compara cada nueva huella de voz contra todos los perfiles de hablantes ya detectados en la conversación, no solo contra el último
- Al terminar la conversación, permite ponerle un nombre real a cada persona detectada
- Recuerda las voces guardadas entre sesiones, para reconocer a la misma persona en conversaciones futuras sin tener que volver a nombrarla
- Modo oscuro, con detección automática de la preferencia del sistema y memoria de la elección
- Auto-scroll de toda la página a medida que llega texto nuevo

## Cómo usarlo

Abre la web publicada en Safari (funciona mejor en iPhone), dale permiso de micrófono, y pulsa "Empezar a escuchar". Se puede añadir a la pantalla de inicio desde el botón de compartir de Safari para que funcione como una app.

## Estado del proyecto

Prototipo en desarrollo activo, probado ya en conversaciones reales. Limitaciones conocidas: Safari no da marcas de tiempo por palabra ni confianza de transcripción, así que no se usan; cortar a mitad de reconocimiento sigue exigiendo reiniciar el motor del navegador, con un pequeño riesgo de perder alguna palabra justo en el punto de corte. La huella de voz es heurística, no un modelo de embeddings entrenado. Pendiente de afinar umbrales con más pruebas reales. Explorando también cómo extenderlo a videollamadas y a conversaciones de grupo grandes.
