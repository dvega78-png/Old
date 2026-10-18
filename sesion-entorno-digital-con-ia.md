# Sesión: Configurar tu entorno de trabajo digital con IA
### De los archivos sueltos a un sistema documentado

**Público:** profesionales y directivos (formación ejecutiva)
**Duración:** 3 horas (hay una versión de 90 minutos al final)
**Formato:** explicación + caso + ejercicio en grupos
**Material necesario:** portátil por grupo; opcionalmente, acceso a un asistente de IA (Claude u otro)

---

## 1. Objetivos de aprendizaje

Al terminar la sesión, los participantes serán capaces de:

1. Diseñar la **arquitectura** de un repositorio documental (quién accede a qué) antes de tocar ninguna herramienta.
2. Aplicar un **método iterativo con IA** para configurar herramientas que no dominan, aprendiendo mientras avanzan.
3. Diagnosticar los **bloqueos típicos** de Microsoft 365 / Google Workspace y entender su causa, no solo el truco para salir.
4. Producir un **documento vivo (.md)** que permita mantener, delegar o migrar su entorno sin depender de la memoria de nadie.

---

## 2. Estructura de la sesión

| Bloque | Contenido | Tiempo |
|---|---|---|
| 0 | Apertura y diagnóstico | 15 min |
| 1 | Principios de un entorno documental sano | 30 min |
| 2 | El método: iterar con IA y documentar | 30 min |
| — | Descanso | 15 min |
| 3 | Caso: Clínica Norte Salud | 20 min |
| 4 | Ejercicio en grupos | 60 min |
| 5 | Puesta en común y cierre | 10 min |

---

## 3. Bloque 0 — Apertura (15 min)

**Pregunta de arranque** (a mano alzada o en un formulario rápido):

> "Piensa en el último contrato importante que compartiste con tu equipo. ¿Dónde está ahora mismo? ¿Quién más tiene una copia? Si mañana dejas la empresa, ¿alguien sabría encontrarlo?"

**Mini-diagnóstico.** Cada participante puntúa de 1 a 5:
- Mis documentos de trabajo están en un espacio común, no en mi ordenador o mi OneDrive/Drive personal.
- Sé quién tiene acceso a la información sensible de mi área.
- Si cambio de ordenador mañana, no pierdo nada ni tardo más de una hora en estar operativo.
- Existe un documento que explica cómo está organizado nuestro entorno.

**Mensaje clave:** la mayoría de organizaciones pequeñas y medianas funcionan con "archivos sueltos compartidos". Funciona hasta el día en que alguien se va, se pierde una versión o una persona ve lo que no debía.

---

## 4. Bloque 1 — Principios (30 min)

### 4.1 Arquitectura antes que herramienta
Antes de abrir SharePoint o Drive, responder en papel:
- ¿Qué niveles de acceso necesito? (Ej.: toda la organización / dirección / cada departamento.)
- ¿Quién pertenece a cada nivel?
- ¿Qué tipo de información va en cada uno?

### 4.2 Permisos por espacio, no por carpeta
- Cada nivel de acceso = **un espacio propio** (un sitio, un canal privado, una unidad compartida).
- Todo lo que hay dentro **hereda** los permisos.
- Dar permisos carpeta a carpeta funciona al principio y se convierte en un caos a los seis meses: nadie sabe quién ve qué.

### 4.3 La información es de la organización, no de las personas
- Los archivos en el OneDrive/Drive personal de alguien dependen de esa persona.
- Mover (no copiar ni descargar y resubir) a espacios comunes conserva versiones y evita duplicados.

### 4.4 Convenciones simples
- Numerar carpetas (`01.`, `02.`…) para fijar el orden.
- Máximo 2–3 niveles de profundidad.
- Nombres cortos y distinguibles (evitar que todos los espacios empiecen igual).

### 4.5 Nube frente a ordenador
Si todo está en la nube, cambiar de ordenador es iniciar sesión. Si algo solo está "en mi escritorio", es un riesgo.

---

## 5. Bloque 2 — El método (30 min)

### 5.1 El ciclo en seis pasos

1. **Partir de una necesidad real**, no de la herramienta. ("Quiero dejar de compartir archivos sueltos", no "quiero aprender SharePoint".)
2. **Diseñar la arquitectura** con la IA como interlocutor: proponer, discutir, ajustar.
3. **Iterar con capturas de pantalla.** Cada vez que algo no aparece o no funciona, se hace captura y se pregunta. Cada bloqueo es una oportunidad para entender cómo funciona el sistema.
4. **Repartir el trabajo:** la IA ejecuta donde puede (con conectores: crear carpetas, mover archivos, comprobar qué existe) y guía donde no puede (permisos, interfaces, decisiones).
5. **Documentar al final en un .md:** estado actual, cómo se hace cada cosa, problemas y soluciones, pendientes, referencia técnica.
6. **Convertirlo en proyecto** (en Claude u otra herramienta): la siguiente sesión empieza con todo el contexto cargado.

### 5.2 Por qué funciona
- **Se aprende haciendo:** el profesional no sigue un curso genérico, resuelve su caso.
- **La IA explica el porqué:** "no lo ves porque los canales privados no aparecen en la portada" enseña más que "haz clic aquí".
- **El .md cierra el ciclo:** convierte una conversación en conocimiento reutilizable, compartible y migrable.

### 5.3 Límites y precauciones
- **Datos sensibles:** no pegar en la IA contenido confidencial que no sea necesario. Las capturas de pantalla pueden mostrar correos, nombres o importes: recortar o tapar antes de compartir.
- **Permisos del conector:** la IA actúa con los permisos de quien la conecta. Revisar qué se le autoriza.
- **La IA puede equivocarse con interfaces:** Microsoft y Google cambian menús con frecuencia. Si una instrucción no coincide con lo que ves, manda captura; no fuerces.
- **Decisiones de negocio:** quién accede a qué lo decide la organización, no la IA.

---

## 6. Bloque 3 — Caso: Clínica Norte Salud (20 min)

> *Caso ficticio basado en una implantación real.*

**Contexto.** Clínica Norte Salud es un grupo sanitario de unas 40 personas en plena fase de crecimiento por adquisiciones. Acaba de contratar Microsoft 365 para empresas. El director financiero, Javier, quiere un repositorio común con tres niveles:
- documentos para toda la organización;
- un espacio solo para el comité de dirección (incluidas las *due diligences* de posibles adquisiciones);
- un espacio por departamento con acceso limitado.

Hasta ahora, cada persona compartía archivos desde su OneDrive. La documentación de una adquisición en curso ("Proyecto Faro") está en el OneDrive de una socia, Marta, en archivos .zip descargados de WeTransfer.

Javier no ha usado nunca SharePoint. Decide resolverlo iterando con un asistente de IA conectado a su cuenta. Durante el proceso se encuentra con estos **incidentes**:

| # | Incidente (lo que dice Javier) |
|---|---|
| 1 | "En SharePoint hay un sitio llamado *Sitio de comunicación* que nadie ha creado. Quiero borrarlo y no me deja." |
| 2 | "Resulta que en Teams ya existe un equipo con un canal *General* y un canal privado *Dirección*. ¿Tengo que crear sitios nuevos en SharePoint?" |
| 3 | "He creado un canal privado para un departamento y no aparece por ningún lado en SharePoint." |
| 4 | "Estoy en el canal y no veo la pestaña de archivos por ninguna parte." |
| 5 | "He añadido un acceso directo al Explorador de Windows y la carpeta sale vacía, pero en SharePoint sí veo los archivos." |
| 6 | "Quiero que todos vean que existe el canal de un departamento, pero que solo entren sus miembros." |
| 7 | "Todos los sitios se llaman *Clínica Norte Salud-…* y en las listas no los distingo." |
| 8 | "En Outlook, dentro de una carpeta, veo muy pocos correos; pero si busco, aparecen todos." |
| 9 | "¿Cómo consigo que la documentación de Proyecto Faro deje de estar en el OneDrive de Marta?" |

---

## 7. Bloque 4 — Ejercicio en grupos (60 min)

Grupos de 3–4 personas. Tres partes.

### Parte A — Diseñar la arquitectura (20 min)
Elegid **uno** de estos dos escenarios:
- **Opción 1:** Clínica Norte Salud.
- **Opción 2:** la organización de uno de los miembros del grupo (sin datos confidenciales).

Entregable: un esquema (papel o pantalla) con:
- los espacios que crearíais y su tipo (canal estándar, canal privado, sitio independiente…);
- quién accede a cada uno;
- 4–6 carpetas principales por espacio, numeradas.

*Pregunta de reflexión:* ¿qué información dejaríais fuera de este sistema y por qué? (Ej.: datos clínicos de pacientes, que suelen requerir su propio sistema y cumplimiento normativo específico.)

### Parte B — Resolver incidentes (20 min)
Cada grupo recibe **tres incidentes** del caso (reparto sugerido: grupo 1 → 1, 4, 7; grupo 2 → 2, 5, 8; grupo 3 → 3, 6, 9).

Para cada incidente:
1. **Causa:** ¿por qué ocurre?
2. **Solución:** ¿qué haríais?
3. **Aprendizaje:** ¿qué os dice sobre cómo funciona la herramienta?

Si hay acceso a IA, usadla como hizo Javier: describid el problema como lo diría él y evaluad críticamente la respuesta. ¿Explica la causa o solo da pasos?

### Parte C — Documentar (20 min)
Con la plantilla del Anexo A, redactad el **.md** de vuestro entorno (Parte A) incluyendo los incidentes que habéis resuelto (Parte B) en la sección de problemas y soluciones.

---

## 8. Bloque 5 — Puesta en común y cierre (10 min)

- Un grupo presenta su arquitectura; los demás la cuestionan: ¿qué pasa si entra una persona nueva en dirección? ¿Y si alguien se va?
- Cada grupo comparte **un** incidente y su aprendizaje.

**Tres ideas para llevarse:**
1. Primero quién ve qué; después la herramienta.
2. Cada bloqueo resuelto es conocimiento: apúntalo.
3. Si no está documentado, depende de la memoria de alguien.

**Reto para la semana siguiente:** aplicar el ciclo a un proceso real propio y traer el .md resultante.

---

## 9. Notas para el profesor — soluciones de los incidentes

| # | Causa | Solución | Aprendizaje |
|---|---|---|---|
| 1 | Es el **sitio raíz** de la organización, creado automáticamente al contratar Microsoft 365. | No borrarlo. Ignorarlo o usarlo como portada/intranet (renombrándolo). | No todo lo que aparece lo ha creado alguien: las plataformas crean estructura por defecto. |
| 2 | Cada equipo de Teams y cada canal privado **ya tiene su propio sitio** de SharePoint con los mismos permisos. | Aprovecharlos: General = toda la organización; canal privado = dirección; un canal privado por departamento. | Teams y SharePoint son dos caras del mismo sistema. Revisar lo que existe antes de crear. |
| 3 | El sitio de un canal privado **se crea la primera vez que alguien abre su pestaña de archivos**, y además no aparece en la portada de SharePoint. | Abrir el canal > pestaña de archivos (*Shared*) > *Open in SharePoint*. Pulsar *Seguir* para que salga en Acceso rápido. | Los espacios privados son "invisibles" por diseño; hay que llegar a ellos desde Teams o por enlace. |
| 4 | El canal está abierto en una **ventana aparte**, que oculta las pestañas. (O la pestaña se llama *Shared* en lugar de *Files*.) | Cerrar la ventana y abrir el canal desde la barra lateral principal. | Las interfaces cambian; describir lo que se ve (captura) es más útil que buscar un nombre concreto. |
| 5 | El acceso directo se creó **desde una subcarpeta**, no desde la raíz de la biblioteca. | Quitar el acceso directo (no borra nada) y crearlo desde la raíz. | Un acceso directo apunta a un sitio concreto; conviene saber a qué. |
| 6 | Un canal privado **solo es visible para sus miembros**. No existe "visible pero cerrado". | Mantenerlo privado y anunciar su existencia en General. | Las herramientas imponen modelos de permisos; a veces se adapta el proceso, no la herramienta. |
| 7 | Los sitios de canales privados se nombran automáticamente *Equipo-Canal*. | Renombrar el sitio (⚙ > Información del sitio) o solo el acceso directo en el Explorador. **Cuidado:** renombrar el sitio principal renombra el equipo de Teams. | Distinguir entre cambios globales (afectan a todos) y locales (solo a mí). Los cambios pueden tardar horas en propagarse. |
| 8 | Una carpeta solo muestra lo guardado en ella (las respuestas van a *Enviados*) y los correos se agrupan por conversación. La búsqueda recorre todas las carpetas. | Ajustar *Configuración > Correo > Organización de mensajes*: agrupar por conversación (no por ramas) y mostrar mensajes de otras carpetas. | "No lo veo" no siempre es "no está": entender el modelo de datos evita pánicos. |
| 9 | La información depende de una persona y está en formato no navegable (.zip). | Descomprimir y **mover** (no descargar y resubir) al espacio de dirección, en una carpeta por proyecto. Confirmar antes que Marta es miembro del espacio de destino. | La información de la organización debe vivir en espacios de la organización. Mover conserva versiones. |

**Consejos de facilitación**
- Si hay participantes que ya dominan Microsoft 365 o Google Workspace, asignarles el rol de "evaluador" de las respuestas de la IA en la Parte B.
- Insistir en la columna **Aprendizaje**: el objetivo no es memorizar trucos, sino entender el modelo de la herramienta.
- En la Parte A, forzar la pregunta de qué pasa cuando alguien entra o sale: revela si la arquitectura es sostenible.

---

## 10. Versión reducida (90 minutos)

| Bloque | Tiempo |
|---|---|
| Apertura (solo la pregunta de arranque) | 5 min |
| Principios (4.1, 4.2, 4.3) | 15 min |
| Método (5.1 y 5.3) | 15 min |
| Caso (presentación rápida) | 10 min |
| Ejercicio: Parte A (15 min) + Parte B con 2 incidentes (15 min) | 30 min |
| Puesta en común y cierre | 15 min |

La Parte C (documentar) se deja como tarea posterior.

---

## Anexo A — Plantilla .md para los participantes

```markdown
# Entorno de trabajo — [Organización / Área]

Última actualización: [fecha]
Responsable: [nombre]

## 1. Objetivo
[Qué problema resuelve este entorno. Una o dos frases.]

## 2. Arquitectura
| Espacio | Tipo | Quién accede | Enlace |
|---|---|---|---|
| | | | |

### Estructura de carpetas
**[Espacio 1]**
- 01.
- 02.

**[Espacio 2]**
- 01.
- 02.

## 3. Cómo se hace
### [Tarea habitual 1: p. ej. dar acceso a una persona nueva]
1.
2.

### [Tarea habitual 2: p. ej. mover archivos desde mi espacio personal]
1.
2.

## 4. Problemas encontrados y soluciones
| Problema | Causa | Solución |
|---|---|---|
| | | |

## 5. Al cambiar de ordenador
1.
2.

## 6. Pendientes
- [ ]
- [ ]

## 7. Referencia técnica
[Identificadores, enlaces, configuraciones que haga falta recordar.]
```

---

## Anexo B — Equivalencias Microsoft 365 / Google Workspace

| Concepto | Microsoft 365 | Google Workspace |
|---|---|---|
| Espacio común de archivos | Sitio de SharePoint / equipo de Teams | Unidad compartida |
| Espacio restringido | Canal privado / sitio privado | Unidad compartida con miembros limitados |
| Archivos personales | OneDrive | Mi unidad |
| Ver en el ordenador | Acceso directo a OneDrive + sincronización | Google Drive para ordenador |
| Mover conservando historial | "Mover a" | "Mover" (a unidad compartida) |
| Conversación del equipo | Canal de Teams | Espacio de Google Chat |
| Portada / intranet | Sitio de comunicación | Google Sites |

---

## Anexo C — Prompt de partida sugerido para los participantes

> "Quiero organizar los documentos de [mi área/organización] en [Microsoft 365 / Google Workspace] para dejar de compartir archivos sueltos. Necesito [niveles de acceso]. No conozco bien la herramienta. Propónme primero una arquitectura (qué espacios y quién accede a cada uno) y explícame el porqué. Después iremos paso a paso: te iré enviando capturas de lo que veo. Cuando terminemos, resume todo en un archivo .md con: estructura, cómo hacer cada cosa, problemas y soluciones, pendientes y referencia técnica."
