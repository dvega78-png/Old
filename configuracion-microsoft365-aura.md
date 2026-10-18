# Configuración Microsoft 365 — Aura Medical Institute SL

Resumen de cómo está organizado el repositorio de documentos en Teams/SharePoint, cómo hacer las tareas habituales y qué queda pendiente. Última actualización: 29/09/2026.

---

## 1. Idea general

El objetivo es dejar de compartir archivos sueltos desde el OneDrive de cada persona y tener un **repositorio común de carpetas** con distintos niveles de acceso.

La regla principal: **los permisos se dan por espacio (canal o sitio), no carpeta por carpeta.** Cada nivel de acceso tiene su propio espacio y todo lo que hay dentro hereda sus permisos. Así es más fácil de mantener y es más difícil que alguien vea lo que no debe.

En Teams, cada equipo y cada canal privado crea automáticamente su propio espacio en SharePoint con los mismos permisos que el equipo o canal.

## 2. Estructura actual

Cuenta: `dvega@auramedicalinstitute.com`
Equipo de Teams: **Aura Medical Institute SL**

| Espacio | Tipo | Quién accede | Sitio SharePoint |
|---|---|---|---|
| General | Canal estándar | Todos los miembros del equipo | `auramedicalinstitute.sharepoint.com/sites/AuraMedicalInstituteSL` |
| Leadership Team | Canal privado | Solo equipo directivo | `auramedicalinstitute.sharepoint.com/sites/AuraMedicalInstituteSL-LeadershipTeam` |
| BRGSDV | Canal privado | Solo sus miembros | `auramedicalinstitute.sharepoint.com/sites/AuraMedicalInstituteSL-BRGSDV` (renombrado a "BRGSDV") |
| Sitio de comunicación | Sitio raíz | Toda la organización | `auramedicalinstitute.sharepoint.com` |

**Sitio de comunicación**: es el sitio raíz que Microsoft crea automáticamente al dar de alta la cuenta. Nadie lo creó a mano y no conviene borrarlo. Se puede ignorar o usar más adelante como portada/intranet (noticias, enlaces).

**All Company** (en Communities de Teams) es para comunicados y conversaciones, no para archivos.

### Carpetas creadas

**General** (dentro de la carpeta "General" de la biblioteca del equipo):
- 01. Políticas y procedimientos
- 02. Formatos y plantillas
- 03. Comunicados
- 04. Recursos compartidos

**Leadership Team** (en la raíz de la biblioteca "Documentos"):
- 01. Due Diligences (una subcarpeta por proyecto; en cada una: Comercial, Financiera, Legal y fiscal, Médica / Operativa)
- 02. M&A y operaciones corporativas
- 03. Consejo y actas
- 04. Finanzas y presupuestos
- 05. Estrategia y plan de negocio
- 06. Contratos y legal

Los números al inicio del nombre fuerzan el orden en lugar del alfabético.

---

## 3. Cómo hacer cada cosa

### Crear un canal (p. ej. para un departamento)
1. En Teams (ordenador), pasar el cursor sobre **Aura Medical Institute SL** > **⋯** > **Add channel**.
2. Nombre del departamento y **Privacy: Private**.
3. **Create** y agregar solo a los miembros del departamento (y a dirección si debe acceder).
4. Si no aparece la opción: **See all your teams** > **⋯** junto al equipo > **Manage team** > pestaña **Channels** > **Add channel**. O probar en **teams.microsoft.com**.
5. Si tampoco aparece "Private": hay que ser **Owner del equipo**. Pedírselo a quien creó el equipo.

Alternativa sin Teams: **SharePoint > Compilar > Sitio > Sitio de grupo**, privacidad **Privado**. Funciona igual para carpetas pero no aparece en la barra lateral de Teams.

Un canal privado **no puede ser visible para todos y cerrado a la vez**: los no miembros no lo ven. Para que la gente sepa que existe, anunciarlo en el canal General.

### Activar el espacio de archivos de un canal nuevo
El sitio de SharePoint de un canal se crea la **primera vez que alguien abre su pestaña de archivos**:
1. En Teams (ventana principal, no ventana aparte), entrar al canal.
2. Pulsar la pestaña **Shared** (junto a *Conversation*), o desplegar **Posts ˅ > Shared**.
3. Pulsar **Open in SharePoint**.

Si el canal está abierto en **ventana aparte** (título "Aura Medical Institute SL | canal"), las pestañas no se ven. Cerrarla y abrir el canal desde la barra lateral.

### Crear carpetas
En Teams: canal > **Shared** > **+ New / + Add** > **Folder**. Si no aparece, **Open in SharePoint** > **+ Crear o cargar** > **Carpeta**.

### Ver archivos del canal en el Explorador de Windows (acceso directo)
1. En SharePoint, ir a la **raíz** de "Documentos" del sitio (sin entrar en ninguna carpeta).
2. Pulsar **Agregar acceso directo a OneDrive**.
3. Aparece en el Explorador en **OneDrive > Shortcuts**.

Si el acceso directo sale vacío, probablemente apunta a una subcarpeta. Quitarlo (OneDrive web > Shortcuts > ⋯ > **Quitar acceso directo**, no borra nada del sitio) y volver a crearlo desde la raíz.

### Mover archivos de OneDrive personal a un canal
- **Usar siempre "Mover a"**, nunca descargar y volver a subir: conserva el historial de versiones y no deja duplicados.
- OneDrive web: seleccionar > **Mover a** > elegir el sitio. Si no aparece en *Reciente*: **Mis archivos > Shortcuts > [sitio]** o **Más lugares…**
- Móvil: la app solo deja elegir destinos dentro de tu OneDrive; usar **Shortcuts > [sitio] > Move here**.
- Explorador de Windows: arrastrar al acceso directo en *Shortcuts* y esperar a que la nube de OneDrive termine de sincronizar.
- El botón **Move here** está en gris hasta que se entra en una carpeta de destino.
- Una vez movidos, los archivos dejan de estar en el OneDrive/ordenador personal y quedan en el sitio compartido.

### Encontrar sitios de canales privados en SharePoint
No aparecen solos en *Descubrir* ni en *Acceso rápido*. Para que aparezcan: entrar una vez desde Teams (**Shared > Open in SharePoint**) y pulsar la estrella **Seguir**. También accesibles desde **OneDrive > Mis archivos > Shortcuts** o **Bibliotecas**.

### Cambiar el nombre de un sitio
- **Nombre del sitio**: dentro del sitio > **⚙ > Información del sitio > Nombre del sitio**. Hace falta ser propietario. Las listas de SharePoint pueden tardar hasta un día en mostrar el nombre nuevo; la cabecera del sitio cambia al momento.
- **Cuidado**: el sitio principal "Aura Medical Institute SL" está ligado al equipo de Teams; renombrarlo cambia también el nombre del equipo.
- **Solo en tu ordenador**: Explorador > OneDrive > Shortcuts > clic derecho en el acceso directo > **Cambiar nombre**. No afecta a nadie más.

### Ver y gestionar miembros de un canal
Barra lateral de Teams > **⋯** junto al canal (no los tres puntos de arriba a la derecha) > **Manage channel** > **Members**. Solo los **Owners** pueden agregar/quitar miembros. Para entrar en un canal privado, la persona debe ser antes miembro del equipo.

### Móvil
- SharePoint móvil: no permite crear sitios (solo consultar, ver archivos y publicar noticias).
- Teams móvil: permite crear canales, pero la opción privada no siempre aparece.
- Para configurar estructura, usar siempre el ordenador.

---

## 4. Outlook (nuevo Outlook)

**Por qué en una carpeta se ven menos correos que en el buscador:**
- Una carpeta solo muestra lo guardado en ella. Tus respuestas van a **Sent Items** y los borradores descartados a **Deleted Items**. El buscador busca en todas las carpetas (la etiqueta a la derecha de cada resultado indica dónde está).
- Los correos se agrupan por conversación; hay que desplegar con la flecha **›**.

**Configuración recomendada** — **⚙ Settings > Email > Message List > Message organisation**:
- Elegir **Group messages by conversation** (antes estaba en "Group messages by branches within conversations", que parte un mismo hilo en varias líneas).
- Alternativa: **Do not group messages** para ver cada correo por separado.
- Más abajo, en **How do you want your reading pane to be organised?**, elegir mostrar todos los mensajes de la conversación y, si aparece, incluir mensajes de otras carpetas.
- Pulsar **Save**.

---

## 5. Al cambiar de ordenador

Todo lo de SharePoint, Teams y OneDrive está en la nube; no se pierde nada. En el ordenador nuevo:
1. Instalar/iniciar sesión en **OneDrive** con `dvega@auramedicalinstitute.com`. Los accesos directos de *Shortcuts* reaparecen solos (los nombres personalizados en el Explorador puede que haya que volver a ponerlos).
2. Instalar **Teams** e iniciar sesión.
3. **Outlook**: la configuración del nuevo Outlook va con la cuenta; revisar igualmente **Message organisation**.
4. Revisar que la nube de OneDrive (junto al reloj) no esté en pausa ni con error.

---

## 6. Pendientes

- [ ] Borrar las carpetas vacías **"Carpeta"** y **"Documentos compartidos"** de la raíz de Leadership Team (después de quitar cualquier acceso directo que apunte a ellas).
- [ ] Conseguir rol de **Owner** en el equipo *Aura Medical Institute SL* y en el canal *Leadership Team*.
- [ ] Comprobar que todos los empleados son miembros del equipo (para que General sea realmente de toda la organización): **⋯ > Manage team > Members**.
- [ ] Comprobar que **Belén Ruiz** es miembro de Leadership Team y enviarle el email con instrucciones para mover la DD de Proyecto LOOK.
- [ ] Archivos de Proyecto LOOK: están como .zip de WeTransfer en el OneDrive de Belén (*01. DUE DILIGENCES/DATAROOM*). Descomprimir y mover el contenido a *Leadership Team > 01. Due Diligences > Proyecto LOOK*.
- [ ] Mover al sitio de Leadership el resto de material de DD (LOOK, Navia, P. Estética) que está en OneDrive personales.
- [ ] Crear los canales privados de cada **departamento** y su estructura de carpetas.
- [ ] Seguir (estrella) los sitios de canales privados para que salgan en *Acceso rápido*.

---

## 7. Referencia técnica (para retomar con Claude)

- Team ID: `c32f6735-5782-4d19-ade5-e6672dd5b826`
- Biblioteca del equipo (General) — driveId: `b!71251V9U-UWLRDWet6mgSeIazJvqHONGhoDh_F7wrhR7c0csQJGCS4Nuzvw7owrr`; carpeta General: `015DPQRW2CWRDH2T4FHBHIWJLYC5PATUDD`
- Biblioteca Leadership Team — driveId: `b!0_JumsxWzUmyjMvmnzAWfkH3cYaAXJpFpRK4xtSneco-l_pLecpIQal1Gi_JYJA-`
- Canal BRGSDV — ID: `19:y4zLMrh3m__sn6H3l2FNce2Jgm4tAvOADsbDKd9PWts1@thread.tacv2`

Truco: si Claude no encuentra el sitio de un canal privado nuevo, crear una carpeta de prueba en él desde SharePoint y pedirle que la busque por nombre; así aparece el driveId.
