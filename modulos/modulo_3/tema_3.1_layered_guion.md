# GUIÓN: TEMA 3.1 (LAYERED ARCHITECTURE)

## FICHA TÉCNICA

- **Duración**: 4 minutos
- **Tono**: Gastronómico.

---

### 00:00 - LA LASAÑA DE SOFTWARE

**[LOCUTOR]**:
Imagina una lasaña.
Tiene capas claras. Pasta, carne, queso, salsa.
No mezclas la carne con el postre.
La arquitectura por capas es igual. Es el diseño más intuitivo que existe.

Arriba del todo, la **Presentación**. El camarero que atiende al cliente. Lo único que sabe hacer es tomar notas y sonreír.
En medio, el **Negocio**. El chef. Él sabe cocinar. Sabe que el filete tarda 10 minutos. No sabe quién se lo va a comer, solo sabe cocinarlo.
Abajo, la **Persistencia**. La despensa. El chef pide "tomates", y la despensa se los da. Al chef no le importa si los tomates vienen del huerto o del supermercado.

---

### 01:15 - SEPARATOIN OF CONCERNS

**[LOCUTOR]**:
La regla sagrada es: El camarero NO cocina. Y la despensa NO sirve mesas.
Si pones sentencias SQL en tu botón de React... has roto la lasaña. Has hecho un revuelto.
Mantén las capas puras.
Así, si mañana cambias MySQL por MongoDB, solo tocas la capa de abajo (Persistencia). El chef (Negocio) ni se entera.

---

### 02:30 - EL SINKHOLE (AGUJERO NEGRO)

**[LOCUTOR]**:
Pero cuidado.
A veces creamos capas por vicio.
Tienes un Controlador que llama a un Servicio que llama a un Repositorio... y ninguno hace nada. Solo pasan el dato.
Es burocracia.
Si el 100% de tu app es CRUD simple (Crear, Leer, Actualizar, Borrar), quizás esta arquitectura es demasiado compleja.
No tengas miedo de simplificar.

---

### 03:40 - CIERRE

**[LOCUTOR]**:
La arquitectura por capas es un clásico por una razón: Funciona. Es fácil de testear y fácil de entender.
Empieza por aquí. Si creces mucho, ya la partirás en microservicios.
Pero una buena lasaña siempre es mejor que un plato de espaguetis enredados.
