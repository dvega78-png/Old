# Copilot vs. Claude Code: guía de privacidad para la UE

Oct 18, 2026 · @David

En privacidad, GitHub Copilot gana en sus planes de empresa y Claude Code gana en el control de lo que hace en tu ordenador; en los planes individuales están prácticamente empatados.

Esta guía compara ambas herramientas usadas desde Visual Studio Code, desde el punto de vista de un usuario en la Unión Europea. Está pensada para personas sin formación en protección de datos: cada sección empieza con un apartado **Conceptos clave** que explica los términos que aparecen después. Al final hay un glosario completo ordenado alfabéticamente.

## Las dos herramientas en una frase

- **GitHub Copilot**: asistente de programación de GitHub (empresa de Microsoft). Sugiere código mientras escribes, responde en un chat y, en "modo agente", puede editar archivos y ejecutar comandos por ti. Por dentro usa modelos de varias empresas (OpenAI, Anthropic, Google, xAI).
- **Claude Code**: asistente de programación de Anthropic. Funciona sobre todo como **agente**: lee tu proyecto, edita archivos y ejecuta comandos en la terminal. Usa los modelos Claude de Anthropic.

## Por qué importa la privacidad aquí

Cuando usas estas herramientas, fragmentos de tu código (y a veces datos, contraseñas o información de clientes que haya en él) salen de tu ordenador y viajan a servidores de otra empresa. Las preguntas que responde esta guía son: ¿quién recibe esos datos, dónde se guardan, cuánto tiempo, para qué se usan y qué protección legal tienes como europeo?

## Resumen en una página

**Conceptos clave**

- **Plan individual (o de consumo)**: la suscripción que contrata una persona a título propio. Copilot Free, Pro y Pro+; Claude Free, Pro y Max.
- **Plan empresarial (o comercial)**: la suscripción que contrata una empresa para sus empleados, con un contrato y garantías distintas. Copilot Business y Enterprise; Claude Team, Enterprise y la API.
- **Opt-out (exclusión voluntaria)**: la opción viene activada por defecto y eres tú quien tiene que desactivarla. Lo contrario es **opt-in**: está desactivada hasta que tú la activas.
- **Residencia de datos**: garantía de que tus datos se procesan y guardan solo en una zona geográfica concreta (por ejemplo, la UE).

**Lo esencial**

- **Planes individuales:** ninguno es privado por defecto. Los dos usan tus datos para entrenar sus modelos salvo que lo desactives (opt-out). En Claude, si no lo desactivas, tus datos se guardan 5 años; si lo desactivas, 30 días.
- **Planes empresariales:** gana Copilot Business/Enterprise. No guarda tus prompts ni sugerencias del editor, ofrece residencia de datos en la UE y GitHub está certificada en el marco legal UE-EE. UU. para transferir datos (DPF). Claude empresarial guarda 30 días por defecto y no tiene región UE propia.
- **Máxima privacidad en la UE:** Copilot Business/Enterprise con residencia UE activada, o Claude Code conectado a Amazon Bedrock o Google Vertex AI en una región europea. En ambos casos hay que configurar bien el agente en tu ordenador.

## 1. Entrenamiento con tus datos

Resultado: empate. En los planes individuales los dos entrenan con tus datos salvo que te excluyas; en los empresariales ninguno entrena.

**Conceptos clave**

- **Modelo de IA**: el "cerebro" del asistente; un programa que ha aprendido a escribir código y texto a partir de enormes cantidades de ejemplos.
- **Entrenar con tus datos**: usar tu código y tus conversaciones como ejemplos para mejorar futuras versiones del modelo. El riesgo es que fragmentos de tu código influyan en lo que el modelo genere para otras personas, y que esos datos se guarden más tiempo.
- **Prompt**: lo que le pides al asistente (tu pregunta o instrucción), junto con el código que la herramienta añade como contexto.
- **Datos de interacción**: todo lo que se intercambia al usar la herramienta: tus prompts, las respuestas, fragmentos de código y contexto (nombres de archivos, estructura del proyecto).
- **Afiliada**: empresa del mismo grupo. Microsoft es la empresa matriz de GitHub.

**GitHub Copilot**

- **Individual (Free, Pro, Pro+):** desde el 24 de abril de 2026 GitHub usa los datos de interacción para entrenar sus modelos salvo que te excluyas. Incluye el contexto alrededor del cursor, comentarios, nombres de archivo y estructura del repositorio. Puede compartirlos con Microsoft, pero no con los proveedores de modelos externos.
  - Dónde desactivarlo: github.com/settings/copilot, apartado "Privacy". Si ya te habías excluido antes, se mantiene.
- **Business y Enterprise:** GitHub no usa estos datos para entrenar.

**Claude Code**

- **Consumo (Free, Pro, Max):** desde la actualización de condiciones de 2025, Anthropic entrena con tus chats y sesiones de Claude Code si el ajuste está activado, y venía activado por defecto. La prensa especializada criticó que el interruptor era poco visible; es una crítica, no una sanción.
  - Dónde desactivarlo: claude.ai/settings/data-privacy-controls.
- **Comercial (Team, Enterprise, API, Bedrock, Vertex):** Anthropic no entrena con tu código ni tus prompts, salvo que tu empresa se apunte voluntariamente a un programa de colaboración.
- **Ojo:** lo que envías con los comandos `/feedback`, `/bug` o `/share` incluye la conversación y el código, y se guarda 5 años aunque hayas desactivado el entrenamiento.

## 2. Retención de datos

Resultado: gana Copilot Business/Enterprise, que no guarda prompts ni sugerencias del editor; Claude empresarial los guarda 30 días.

**Conceptos clave**

- **Retención**: cuánto tiempo guarda el proveedor tus datos en sus servidores. Cuanto menos tiempo, menos riesgo si hay una filtración o una petición judicial.
- **Zero Data Retention (ZDR, retención cero)**: el proveedor procesa tu petición y la borra inmediatamente, sin guardarla.
- **Telemetría / datos de uso**: estadísticas sobre cómo usas la herramienta (cuántas sugerencias aceptas, errores, tiempos), normalmente sin tu código.
- **Transcripción local**: copia de tus conversaciones que la herramienta guarda en tu propio ordenador.
- **Covered Models**: los modelos más potentes de Anthropic (clase Mythos/Fable), sometidos a normas especiales de seguridad.

| Dato | Copilot Business/Enterprise | Copilot Free/Pro/Pro+ | Claude Free/Pro/Max | Claude Team/Enterprise/API |
| --- | --- | --- | --- | --- |
| Prompts y sugerencias en el editor | No se guardan | Depende de tus ajustes; con entrenamiento activado se usan para entrenar | 30 días (entrenamiento desactivado) / 5 años (activado) | 30 días |
| Otros accesos (web, móvil, CLI) | 28 días | — | — | — |
| Datos de uso | 2 años | 2 años | Métricas sin código ni prompts | Igual |
| Retención cero (ZDR) | Por defecto en el editor | No | No disponible | Solo cuentas Enterprise aprobadas; no para Covered Models |
| Copia local | — | — | Carpeta `~/.claude/projects/`, texto sin cifrar, 30 días (ajustable con `cleanupPeriodDays`) | Igual |

- **Covered Models:** desde el 9 de junio de 2026, Anthropic guarda 30 días los prompts y respuestas de estos modelos en todas las plataformas (incluidas Bedrock y Vertex), aunque tengas un acuerdo de retención cero.
- **Sin confirmar:** GitHub tiene un acuerdo de retención cero con Anthropic, pero si Copilot ofrece un Covered Model es probable que se aplique igualmente la regla de 30 días. GitHub no lo ha confirmado.

## 3. Residencia de datos en la UE

Resultado: Copilot ofrece residencia UE como parte del producto; Claude Code solo la consigue si lo conectas a Amazon Bedrock o Google Vertex AI en Europa.

**Conceptos clave**

- **Inferencia**: el momento en que el modelo procesa tu petición y genera la respuesta. "Inferencia en la UE" significa que ese cálculo ocurre en servidores europeos.
- **Residencia de datos**: compromiso de que tus datos se procesan y almacenan solo dentro de una región. Reduce los riesgos legales de enviar datos fuera de la UE.
- **EU Data Boundary**: el perímetro de Microsoft que agrupa los países de la UE y de la AELC (Islandia, Liechtenstein, Noruega, Suiza).
- **GitHub Enterprise Cloud con residencia de datos (GHE.com)**: versión de GitHub para empresas alojada en la región que elijas.
- **Amazon Bedrock / Google Vertex AI**: servicios en la nube de Amazon y Google que permiten usar modelos de IA (incluido Claude) dentro de tu propia cuenta en esas nubes, eligiendo la región.
- **Hiperescalador**: gran proveedor de nube (Amazon Web Services, Google Cloud, Microsoft Azure).
- **Región / perfil de inferencia `eu.`**: conjunto de centros de datos europeos de Amazon entre los que se reparte el trabajo. Garantiza Europa, no una ciudad concreta.

**GitHub Copilot**

- Desde el 13 de abril de 2026 ofrece residencia en EE. UU. o en la UE. Toda la inferencia, los registros (logs) y la telemetría se quedan en la región.
- Cubre el modo agente, las sugerencias, el chat, la revisión de código y la CLI.
- **Requisitos y limitaciones:**
  - Necesitas GitHub Enterprise Cloud con residencia de datos (GHE.com) y activar la política "Restrict Copilot to data residency compliant models".
  - Cuesta un 10 % más por petición premium.
  - Los modelos Gemini (Google) no están disponibles con residencia.
  - Los planes Free, Pro y Pro+ no tienen residencia UE.

**Claude Code**

- La API de Anthropic solo permite elegir "global" o "us" (EE. UU.); no hay región UE. Claude Team/Enterprise tampoco la ofrece.
- Para quedarte en Europa, conéctalo a:
  - **Amazon Bedrock**, con el perfil `eu.` (Fráncfort, Irlanda, París, Estocolmo, Milán, España, Zúrich; también Londres, que no es UE).
  - **Google Vertex AI**, con las regiones europe-west1, europe-west4 o la multirregión UE.
- Se activa con la variable `CLAUDE_CODE_USE_BEDROCK=1` o `CLAUDE_CODE_USE_VERTEX=1`.
- **Cuidado:** si no defines `AWS_REGION`, Claude Code usa por defecto us-east-1, que está en EE. UU.

## 4. RGPD: contratos, transferencias y subencargados

Resultado: ventaja para Copilot por su contrato de protección de datos público y su certificación en el DPF; Anthropic compensa en parte con una entidad irlandesa como contraparte.

**Conceptos clave**

- **RGPD (GDPR en inglés)**: Reglamento General de Protección de Datos de la UE. Regula cómo se tratan los datos personales de personas en Europa.
- **Dato personal**: cualquier información sobre una persona identificable (nombre, email, IP, datos de clientes en una base de datos de prueba…). El código en sí no suele serlo, pero puede contenerlos.
- **Responsable del tratamiento**: quien decide para qué y cómo se usan los datos.
- **Encargado del tratamiento**: quien trata los datos por cuenta del responsable, siguiendo sus instrucciones (por ejemplo, el proveedor de IA de tu empresa).
- **Subencargado**: empresa a la que el encargado subcontrata parte del trabajo (por ejemplo, el proveedor de nube o del modelo).
- **DPA (Data Processing Agreement / Acuerdo de tratamiento de datos)**: contrato obligatorio por el RGPD entre una empresa y su encargado, que fija qué se puede hacer con los datos.
- **Transferencia internacional**: enviar datos personales fuera del Espacio Económico Europeo. Solo es legal con una base jurídica.
- **DPF (EU-US Data Privacy Framework)**: acuerdo entre la UE y EE. UU. que permite enviar datos a empresas estadounidenses certificadas. Es la base más sencilla.
- **SCC (Cláusulas Contractuales Tipo)**: cláusulas aprobadas por la Comisión Europea que se añaden al contrato para permitir la transferencia cuando no hay DPF.
- **noyb**: asociación europea de defensa de la privacidad que suele litigar contra los acuerdos de transferencia de datos.
- **EDPB**: Comité Europeo de Protección de Datos, que reúne a las autoridades de protección de datos de la UE.

**GitHub**

- Tiene un DPA público que cubre Copilot.
- Las transferencias a EE. UU. se amparan en su certificación en el DPF y/o en SCC.
- **Modelos de terceros:** Copilot envía tus peticiones a distintos proveedores según el modelo que elijas:
  - OpenAI, alojado en Azure, con retención cero.
  - Anthropic, alojado en AWS, Anthropic y Google Cloud, con retención cero en funciones generales (no siempre en las beta).
  - Google Gemini, en Google Cloud, con compromiso de no entrenar.
  - xAI y modelos abiertos, también con retención cero.
- Consecuencia: si eliges Claude dentro de Copilot, tu código puede llegar a Anthropic en EE. UU., pero bajo el contrato de GitHub.

**Anthropic**

- En el EEE, Reino Unido y Suiza, la empresa responsable es **Anthropic Ireland, Limited** (Dublín). En los contratos comerciales también, con ley irlandesa y DPA con SCC.
- Según el registro oficial, Anthropic **no está** en el DPF (algunas fuentes dicen lo contrario); depende de las SCC.
- En los planes de consumo **no hay DPA**: no son adecuados para tratar datos personales de tu empresa.

**Estado del DPF**

- Tras la sentencia del Tribunal Supremo de EE. UU. *Trump v. Slaughter* (29 de junio de 2026), noyb pidió retirar el DPF y anunció una demanda. El EDPB pidió a la Comisión que evaluara su impacto.
- A mediados de octubre de 2026 el DPF sigue en vigor y no consta ninguna demanda presentada. La ventaja de GitHub es real pero frágil.

## 5. Qué sale de tu ordenador y cómo controlarlo

Resultado: Claude Code da más control sobre lo que el agente puede leer y enviar; la exclusión de contenido de Copilot no funciona en el modo agente del editor.

**Conceptos clave**

- **Agente**: modo en que la IA no solo sugiere, sino que actúa: abre y edita archivos, ejecuta comandos y decide qué leer. Por eso puede enviar al proveedor más cosas de las que imaginas (por ejemplo, un archivo de contraseñas).
- **Contexto**: el código y la información que la herramienta envía junto a tu pregunta para que el modelo entienda tu proyecto.
- **TLS**: el cifrado que protege los datos mientras viajan por internet (el mismo del candado del navegador).
- **Variable de entorno**: un ajuste que se configura en el sistema o la terminal (por ejemplo, `DISABLE_TELEMETRY=1`) para cambiar el comportamiento de un programa.
- **Archivo `.env`**: archivo típico donde los proyectos guardan contraseñas y claves; nunca debería enviarse a una IA.
- **Reglas de denegación (deny)**: lista de archivos o acciones que el agente tiene prohibido usar.
- **Sandbox**: "caja de arena"; un entorno aislado donde los comandos se ejecutan sin poder tocar el resto del sistema.
- **Ajustes gestionados (managed settings)**: configuración que impone la empresa y que el empleado no puede cambiar.
- **Exclusión de contenido (content exclusion)**: función de Copilot que impide que ciertos archivos o repositorios se envíen como contexto.
- **CLI**: interfaz de línea de comandos; usar la herramienta desde la terminal en lugar de desde el editor.

**Claude Code**

- Todo lo que lee el agente viaja cifrado (TLS 1.2 o superior) al proveedor del modelo.
- **Desactivar el tráfico no esencial:**
  - Métricas de uso (sin código ni prompts): `DISABLE_TELEMETRY=1`.
  - Informes de errores (se envían a un tercero, con secretos ocultos): `DISABLE_ERROR_REPORTING=1`.
  - Comando `/feedback`: `DISABLE_FEEDBACK_COMMAND=1`; encuestas: `CLAUDE_CODE_DISABLE_FEEDBACK_SURVEY=1`.
  - Todo a la vez: `CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC=1`.
- Con Bedrock o Vertex, métricas, errores y feedback vienen **desactivados por defecto**.
- **Excepción:** al consultar páginas web, Claude Code envía el nombre del dominio a Anthropic para comprobar su seguridad, incluso con Bedrock o Vertex. Se desactiva con `skipWebFetchPreflight: true`.
- **Controlar al agente:**
  - Reglas deny, por ejemplo `Read(**/.env)` para que no lea contraseñas.
  - Sandbox del sistema operativo para los comandos, que también bloquea un `cat .env`.
  - `managed-settings.json` para que la empresa imponga las reglas.
  - Límite: una regla `Read` por sí sola no impide leer el archivo con un comando de terminal fuera del sandbox.

**GitHub Copilot**

- Envía el contexto del editor (archivo actual, archivos abiertos, fragmentos relevantes) y, en modo agente, lo que el agente lea o ejecute.
- La **exclusión de contenido** (solo Business/Enterprise) funciona en el autocompletado y el chat normal, pero **no en los modos Agent y Edit** de VS Code.
- Desde septiembre de 2026, la app de Copilot y la CLI sí respetan la exclusión de contenido; el modo agente del editor sigue sin hacerlo.
- La telemetría del editor se controla con el ajuste `telemetry.telemetryLevel` de VS Code; el entrenamiento, en tu cuenta de GitHub.

## 6. Controles empresariales y certificaciones

Resultado: empate en certificaciones; Copilot destaca en gobierno integrado con GitHub y residencia UE, y Claude en el control del agente.

**Conceptos clave**

- **Certificación**: auditoría independiente que confirma que una empresa cumple un estándar de seguridad o gestión.
- **SOC 2 Type II**: informe de auditoría estadounidense que revisa durante meses si los controles de seguridad de un proveedor funcionan de verdad (Type I solo revisa su diseño en un momento dado).
- **ISO 27001**: norma internacional de gestión de la seguridad de la información.
- **ISO 27701**: ampliación de la ISO 27001 centrada en la privacidad.
- **ISO/IEC 42001**: norma internacional para gestionar de forma responsable los sistemas de inteligencia artificial.
- **HIPAA / BAA**: ley estadounidense de datos sanitarios y el contrato que exige; poco relevante en Europa.
- **Registro de auditoría (audit log)**: historial de quién hizo qué y cuándo, útil para investigar incidentes.
- **SIEM / OpenTelemetry**: herramientas y formato estándar para enviar esos registros al sistema de seguridad de la empresa.
- **Indemnización por propiedad intelectual**: el proveedor se compromete a defenderte si te demandan porque el código generado copia código protegido.

| Control | Copilot Business/Enterprise | Claude Team/Enterprise / API |
| --- | --- | --- |
| Certificaciones | SOC 1/2 Type II/3, ISO 27001, ISO 27701, ISO 42001, CSA STAR, PCI DSS | SOC 2 Type I y II, ISO 27001:2022, ISO 42001:2023, configuración HIPAA con BAA |
| Políticas centralizadas | Políticas de empresa/organización para modelos y funciones; bloquear Copilot Free | Ajustes gestionados (MDM, servidor), MCP gestionado, analíticas |
| Exclusión de archivos | Exclusión de contenido (no en modos Agent/Edit) | Reglas deny y sandbox gestionados |
| Auditoría | Audit log de GitHub | Analíticas y OpenTelemetry exportable a SIEM |
| Indemnización por PI | Sí (con filtro de código público) | Sí, en términos comerciales |
| Residencia UE | Nativa (GHE.com) | Solo vía Bedrock/Vertex |

## 7. Contexto regulatorio en la UE

Resultado: ninguna autoridad europea ha sancionado ni investigado formalmente a Copilot ni a Claude Code; las obligaciones del AI Act recaen en los proveedores, no en ti.

**Conceptos clave**

- **AI Act (Reglamento de Inteligencia Artificial)**: ley de la UE que regula la IA según su nivel de riesgo.
- **IA de propósito general (GPAI)**: modelos que sirven para muchas tareas distintas, como los de OpenAI o Anthropic. Tienen obligaciones específicas de transparencia y seguridad.
- **Código de Buenas Prácticas**: guía voluntaria de la Comisión Europea para que los proveedores de GPAI demuestren que cumplen el AI Act.
- **Oficina de IA (AI Office)**: órgano de la Comisión Europea que supervisa a los proveedores de GPAI.
- **Uso de alto riesgo**: usos de la IA que el AI Act regula con más dureza (por ejemplo, selección de personal o crédito). Programar con un asistente no lo es, en principio.
- **Autoridad de protección de datos**: organismo nacional que vigila el cumplimiento del RGPD (en España, la AEPD).
- **Directiva ePrivacy**: norma de la UE sobre privacidad en comunicaciones electrónicas, como el acceso a información guardada en el dispositivo del usuario.

**AI Act**

- Anthropic, Microsoft y OpenAI firmaron el Código de Buenas Prácticas (publicado el 10 de julio de 2025).
- Las obligaciones para estos modelos se aplican desde el 2 de agosto de 2025. Desde el 2 de agosto de 2026 la Oficina de IA puede investigar y multar (hasta 15 M€ o el 3 % de la facturación mundial). Los modelos lanzados antes tienen hasta el 2 de agosto de 2027.

**Autoridades de protección de datos**

- No consta ninguna investigación ni decisión contra GitHub Copilot ni contra Claude.
- El 27 de abril de 2026 se presentó en Malta una queja sobre Claude Desktop basada en la Directiva ePrivacy. Según fuentes secundarias, la autoridad maltesa la rechazó el 8 de mayo de 2026 por falta de competencia territorial.
- Los cambios a opt-out de ambas empresas han recibido críticas, pero no sanciones.

## Tabla resumen

| Aspecto | Ventaja | Motivo |
| --- | --- | --- |
| Entrenamiento (individual) | Empate | Ambos con opt-out por defecto |
| Entrenamiento (empresa) | Empate | Ninguno entrena |
| Retención con entrenamiento activado (individual) | Copilot (ligera) | Claude guarda 5 años |
| Retención en el editor (empresa) | Copilot | Cero retención frente a 30 días |
| Retención cero (ZDR) | Copilot | Por defecto en el editor; en Anthropic solo aprobada y sin Covered Models |
| Residencia UE | Copilot (producto); Claude iguala vía Bedrock/Vertex | GHE.com con política de residencia |
| Transferencias (DPF) | Copilot | GitHub certificada; Anthropic solo SCC |
| Entidad europea | Claude (ligera) | Anthropic Ireland como responsable y contraparte |
| Telemetría local | Claude Code | Variables documentadas; apagada por defecto en Bedrock/Vertex |
| Control del agente sobre archivos | Claude Code | Reglas deny, sandbox y ajustes gestionados |
| Certificaciones | Empate | Ambos SOC 2 Type II, ISO 27001, ISO 42001 |
| Cadena de subencargados | Claude vía Bedrock/Vertex (más corta) | Copilot reparte entre OpenAI, Anthropic, Google, xAI |

## Recomendaciones

1. **Si usas un plan individual:**
   - Desactiva hoy el entrenamiento: en GitHub, Settings → Copilot → Privacy; en Claude, claude.ai/settings/data-privacy-controls. En Claude, esto baja la retención de 5 años a 30 días.
   - No uses `/feedback` ni `/bug` en Claude con código sensible: se guarda 5 años.
   - No uses planes individuales con código de clientes que contenga datos personales: no tienen DPA.
2. **Si trabajas en una empresa con requisitos RGPD estrictos:**
   - Opción más sencilla: Copilot Business/Enterprise sobre GHE.com con residencia UE activada, y Copilot Free bloqueado en la organización.
   - Si preferís Claude Code: conectadlo a Bedrock (perfil `eu.` y `AWS_REGION` en una región UE) o a Vertex (europe-west1/4). Así la telemetría va apagada y el tratamiento queda bajo el DPA de AWS o Google.
3. **Configura el agente en cualquier caso:**
   - Claude Code: `managed-settings.json` con reglas deny para `.env`, `~/.ssh` y `~/.aws`, sandbox activado, `CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC=1` y `skipWebFetchPreflight` si bloqueáis api.anthropic.com.
   - Copilot: no confíes en la exclusión de contenido en modo agente. Deja los secretos fuera del proyecto o usa contenedores de desarrollo (dev containers).
4. **Revisa qué modelo eliges.** En Copilot, cambiar a Claude o Gemini cambia quién recibe los datos, y Gemini no está disponible con residencia UE. En Claude, evita los Covered Models si necesitas retención cero.
5. **Documenta la base legal de la transferencia en tu evaluación de impacto (DPIA).** El DPF está en revisión y Anthropic depende de las SCC.

## Advertencias

- Algunos datos vienen de análisis de terceros o de fuentes que se contradicen: las certificaciones de Copilot, la exclusión de contenido en la CLI y la app, la queja en Malta y si Anthropic está en el DPF. Compruébalos en el GitHub Copilot Trust Center, trust.anthropic.com y dataprivacyframework.gov antes de firmar ningún contrato.
- GitHub no publica una cifra clara de retención de prompts para los planes individuales; depende de tus ajustes.
- Que la regla de 30 días de los Covered Models se aplique dentro de Copilot es una deducción razonable, no algo confirmado por GitHub.
- Ambas empresas han cambiado sus políticas varias veces entre 2025 y 2026. Revisadlas periódicamente.
- Esta guía no es asesoramiento jurídico; para decisiones contractuales, consultad con vuestro delegado de protección de datos (DPO).

## Glosario

| Término | Qué significa |
| --- | --- |
| Afiliada | Empresa del mismo grupo (Microsoft respecto a GitHub). |
| Agente | Modo en que la IA actúa por sí misma: lee y edita archivos y ejecuta comandos. |
| AI Act | Reglamento europeo que regula la inteligencia artificial según su riesgo. |
| Amazon Bedrock | Servicio de Amazon para usar modelos de IA (incluido Claude) en tu cuenta de AWS, eligiendo región. |
| API | Forma de acceder a un servicio desde otros programas; la vía "técnica" de usar Claude. |
| Audit log | Registro de quién hizo qué y cuándo. |
| CLI | Uso de una herramienta desde la terminal (línea de comandos). |
| Contexto | Código e información que se envían junto a tu pregunta. |
| Covered Models | Modelos más potentes de Anthropic, con retención obligatoria de 30 días. |
| Datos de interacción | Prompts, respuestas, fragmentos de código y contexto intercambiados con la herramienta. |
| Dato personal | Cualquier información sobre una persona identificable. |
| DPA | Contrato obligatorio entre una empresa y quien trata datos por su cuenta. |
| DPF | Acuerdo UE-EE. UU. que permite enviar datos a empresas estadounidenses certificadas. |
| DPIA | Evaluación de impacto en protección de datos que exige el RGPD para tratamientos de riesgo. |
| DPO | Delegado de protección de datos de una organización. |
| EDPB | Comité Europeo de Protección de Datos. |
| Encargado del tratamiento | Quien trata datos por cuenta de otro, siguiendo sus instrucciones. |
| Entrenamiento | Usar datos para mejorar un modelo de IA. |
| Exclusión de contenido | Función de Copilot para impedir que ciertos archivos se envíen. |
| GHE.com | GitHub Enterprise Cloud alojado en la región que elijas. |
| Google Vertex AI | Servicio de Google Cloud para usar modelos de IA (incluido Claude) eligiendo región. |
| GPAI | IA de propósito general: modelos para muchas tareas distintas. |
| Hiperescalador | Gran proveedor de nube (AWS, Google Cloud, Azure). |
| Indemnización por PI | Compromiso del proveedor de defenderte si el código generado infringe derechos de autor. |
| Inferencia | El cálculo que hace el modelo para responder a tu petición. |
| ISO 27001 / 27701 / 42001 | Normas de seguridad de la información, privacidad y gestión de IA. |
| Managed settings | Configuración impuesta por la empresa que el usuario no puede cambiar. |
| Modelo de IA | Programa que ha aprendido a generar texto y código. |
| noyb | Asociación europea de defensa de la privacidad. |
| Opt-in / opt-out | Activado solo si tú lo activas / activado salvo que tú lo desactives. |
| Plan comercial | Suscripción contratada por una empresa, con contrato y garantías propias. |
| Plan de consumo | Suscripción contratada por una persona a título individual. |
| Prompt | Lo que le pides al asistente. |
| Reglas deny | Lista de archivos o acciones prohibidas para el agente. |
| Residencia de datos | Garantía de que los datos se procesan y guardan solo en una región. |
| Responsable del tratamiento | Quien decide para qué y cómo se usan los datos. |
| Retención | Tiempo que el proveedor guarda tus datos. |
| RGPD | Reglamento General de Protección de Datos de la UE. |
| Sandbox | Entorno aislado donde se ejecutan comandos sin tocar el resto del sistema. |
| SCC | Cláusulas Contractuales Tipo de la Comisión Europea para transferir datos fuera de la UE. |
| SIEM | Sistema que centraliza los registros de seguridad de la empresa. |
| SOC 2 Type II | Auditoría que comprueba durante meses que los controles de seguridad funcionan. |
| Subencargado | Empresa a la que el encargado subcontrata parte del tratamiento. |
| Telemetría | Estadísticas de uso que la herramienta envía al proveedor. |
| TLS | Cifrado que protege los datos en tránsito por internet. |
| Transferencia internacional | Envío de datos personales fuera del Espacio Económico Europeo. |
| Variable de entorno | Ajuste del sistema o la terminal que cambia el comportamiento de un programa. |
| ZDR | Retención cero: los datos se borran nada más procesarlos. |

## Fuentes

**Oficiales: GitHub**

- [Cambios en el uso de datos de interacción de Copilot](https://github.blog/news-insights/company-news/updates-to-github-copilot-interaction-data-usage-policy/)
- [Residencia de datos de Copilot en EE. UU. y la UE](https://github.blog/changelog/2026-04-13-copilot-data-residency-in-us-eu-and-fedramp-compliance-now-available/)
- [Copilot con residencia de datos (documentación)](https://docs.github.com/en/enterprise-cloud@latest/admin/data-residency/github-copilot-with-data-residency)
- [Alojamiento de modelos en Copilot](https://docs.github.com/en/copilot/reference/ai-models/model-hosting)
- [Exclusión de contenido](https://docs.github.com/en/copilot/concepts/context/content-exclusion)
- [Declaración de privacidad de GitHub](https://docs.github.com/site-policy/privacy-policies/github-privacy-statement)
- [Acuerdo de protección de datos de GitHub (PDF)](https://assets.ctfassets.net/8aevphvgewt8/DaflLjyuIt6un69xg3n6W/375560a9e93004190548b6c581b81ef3/GITHUB-202410-GitHubDataProtectionAgreement.pdf)
- [Planes de Copilot](https://github.com/features/copilot/plans)

**Oficiales: Anthropic**

- [Actualización de los términos de consumo](https://www.anthropic.com/news/updates-to-our-consumer-terms?os=0)
- [Uso de datos en Claude Code](https://code.claude.com/docs/en/data-usage)
- [Referencia de ajustes de Claude Code](https://code.claude.com/docs/en/settings-reference)
- [Retención de datos de la API](https://platform.claude.com/docs/en/manage-claude/api-and-data-retention)
- [Residencia de datos de la API](https://platform.claude.com/docs/en/manage-claude/data-residency)
- [Claude en Amazon Bedrock](https://platform.claude.com/docs/en/build-with-claude/claude-in-amazon-bedrock)
- [Retención para Covered Models](https://support.claude.com/en/articles/15425996-data-retention-practices-for-covered-models)
- [Certificaciones de Anthropic](https://privacy.claude.com/en/articles/10015870-what-certifications-has-anthropic-obtained)

**Regulación y contexto**

- [Código de Buenas Prácticas GPAI (Comisión Europea)](https://digital-strategy.ec.europa.eu/en/policies/gpai-code-practice)
- [Aplicación del capítulo V del AI Act](https://artificialintelligenceact.eu/enforcement-of-chapter-v-under-the-eu-ai-act/)
- [noyb sobre las transferencias UE-EE. UU.](https://noyb.eu/en/us-supreme-court-just-blew-eu-us-data-transfers)
- [EDPB y la revisión del DPF tras Slaughter](https://www.gblock.app/articles/edpb-eu-us-data-privacy-framework-review-slaughter-2026)

**Análisis de terceros**

- [Copilot con residencia de datos en Europa (Jesse Houwing)](https://jessehouwing.net/github-copilot-now-with-data-residency-in-europe/)
- [Claude en AWS al estilo UE](https://cloud2.net/field-notes/cloud/claude-on-aws-the-eu-way/)
- [¿Es la API de Claude conforme al RGPD?](https://www.januscompliance.co.uk/blog/is-the-claude-api-gdpr-compliant-2026)
- [Seguridad en Claude Code (DataCamp)](https://www.datacamp.com/tutorial/claude-code-security)
- [Exclusión de contenido de Copilot en cuatro capas](https://blog.cloud-eng.nl/2026/03/13/copilot-content-exclusions-four-layers/)
