# GUIÓN: TEMA 3.2 (MICROKERNEL)

## FICHA TÉCNICA

- **Duración**: 4 minutos
- **Tono**: Ingenieril.

---

### 00:00 - EL TELÉFONO MÓVIL

**[LOCUTOR]**:
Tu teléfono viene de fábrica con lo básico: Llamar, Contactos, Ajustes. Ese es el **Core**.
Pero tú quieres más. Quieres WhatsApp, Spotify, Candy Crush.
Instalas Apps. Esas Apps son **Plugins**.
El sistema operativo (Android/iOS) actúa como el Microkernel. Provee los servicios base (GPS, Cámara, Pantalla) a los plugins.

---

### 01:10 - ENCHUFAR Y LISTO

**[LOCUTOR]**:
La belleza de esta arquitectura es la extensibilidad.
Los creadores de Android no tuvieron que programar Spotify.
Simplemente crearon una API pública ("Aquí tienes cómo sacar sonido") y dejaron que otros innovaran.
Si estás creando un software empresarial complejo... ¿por qué intentas programar todos los casos de uso tú solo?
Crea un Core sólido y permite que otros equipos (o terceros) programen "Add-ons" para funcionalidades específicas.

---

### 02:20 - EL REGISTRO DE PLUGINS

**[LOCUTOR]**:
El Core necesita saber quiénes son los invitados.
Necesita un "Plugin Registry". Una lista VIP.
Cuando arrancas la app, el Core mira el registro, carga los plugins encontrados, y los conecta.
Es vital que el Core no dependa de los Plugins.
Si borras Spotify, el teléfono sigue funcionando.
La dependencia va en una sola dirección: Plugin -> Core. Nunca al revés.

---

### 03:30 - CIERRE

**[LOCUTOR]**:
Usa Microkernel cuando no sepas qué va a necesitar el usuario en el futuro.
Eclipse, VS Code, Jira, WordPress... todos son Microkernels.
Su éxito no es su código base, es su ecosistema de plugins.
Construye plataformas, no solo aplicaciones.
