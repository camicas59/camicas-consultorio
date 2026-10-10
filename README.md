# Camicas · Consultorio

Agenda, pacientes y economía para un consultorio individual. Versión violeta, con detalles florales discretos y mensajes de bienvenida opcionales.

**Abrir desde el celular:** https://camicas59.github.io/camicas-consultorio/

El diseño prioriza el uso táctil: navegación inferior, formularios de una columna, controles cómodos y márgenes para la zona segura del teléfono. Los gráficos se adaptan al ancho disponible. Se verificó desde 320 píxeles de ancho.

## Archivos

- `index.html`: aplicación completa como página inicial.
- `camicas-v2.html`: la misma aplicación en un archivo HTML independiente.
- `manifest.webmanifest`, íconos PNG y SVG: nombre, apariencia e ícono para la pantalla de inicio de iPhone y Android.
- `welcome-sources.md`: fuentes y distinción entre citas y recordatorios propios.
- `.nojekyll`: sirve el HTML como sitio estático sin procesamiento adicional.
- `.gitignore`: excluye respaldos, CSV y archivos locales de trabajo.

Los dos HTML son idénticos. El uso local no requiere compilación ni paquetes. La conexión opcional con Google Forms requiere internet y autorización de Google. El código no contiene pacientes reales ni registros de prueba.

## Apariencia y bienvenida

La paleta combina violeta suave y lavanda. El modo oscuro mantiene esa familia de colores. Las flores acompañan los controles habituales; no hay botón de pausa ni temporizadores.

Al abrirse o volver a la aplicación, puede aparecer una bienvenida encima de la pantalla. Hay que cerrarla con la X o **Entrar a Camicas**. Se muestra como máximo dos veces por día y con al menos seis horas entre mensajes; no queda como una tarjeta del inicio. El cartel muestra la cita y su autor, con la X y **Entrar a Camicas** como únicas acciones. El límite se cuenta en el navegador del celular. La preferencia general se administra desde **Más**.

La biblioteca incluye **80 mensajes: 20 citas breves verificadas y 60 recordatorios originales de Camicas** sobre psicología, logoterapia, psicotrauma y atención al presente. Las citas muestran el autor y comillas; los recordatorios llevan la firma Camicas y no usan comillas. Las citas originalmente en inglés se presentan en español, con una traducción cercana. Las [fuentes y los criterios de selección](welcome-sources.md) se conservan en la guía, sin recargar el cartel.

La biblioteca se mezcla en rondas: ningún mensaje vuelve a salir hasta completar la ronda. La selección pendiente se conserva al cerrar la aplicación.

## Ícono en el celular

El ícono propio combina violeta, una c blanca y una flor discreta. Se incluyen los tamaños de iPhone y Android, incluido el formato adaptable.

En iPhone: abrí el enlace en Safari, elegí **Compartir → Agregar a la pantalla de inicio** y activá **Abrir como app web** si aparece. En Android: abrí el enlace en Chrome y elegí **Agregar a la pantalla principal** o **Instalar** si el navegador ofrece esa opción.

Agregá primero el acceso nuevo y comprobá tus registros. Si el acceso anterior tiene datos cargados, exportá una copia desde Más antes de quitarlo; distintos modos del navegador pueden usar almacenamientos separados. El ícono no agrega sincronización ni funcionamiento sin internet a la conexión de Forms.

## Acceso directo y privacidad

Camicas abre sin contraseña propia ni bloqueo al salir. Los registros se guardan localmente sin cifrado de Camicas y no se envían a GitHub. El bloqueo y el acceso al dispositivo se administran en el celular.

Si este navegador contiene un guardado cifrado de la versión anterior, la pantalla inicial permite ingresar su contraseña una sola vez, revisar las cantidades y recuperar los registros para usar el acceso directo. El contenedor cifrado anterior se conserva; una clave incorrecta o un error de almacenamiento no lo elimina. Si hay otra base local, se conservan ambas sin reemplazo automático.

Las nuevas copias completas son JSON sin contraseña. Se pueden importar JSON antiguos y copias cifradas: estas últimas siguen necesitando su contraseña anterior para leerlas. En Más se puede revisar e importar el guardado cifrado anterior con una vista previa y respaldo del estado actual antes de reemplazarlo.

Se mantiene la política de seguridad del contenido con hash del script propio, bloqueo de atributos ejecutables, conexiones limitadas a Google Forms e Identity y política no-referrer. Los permisos de Google permanecen solo en memoria. GitHub protege la cuenta y el código, no el guardado del celular. No se suben pacientes, turnos, economía ni respaldos al repositorio.

[Paso a paso de acceso y respaldo](security-guide.md).

## Funciones

- Inicio con próximos turnos, indicadores, cobros y recordatorios administrativos.
- Agenda diaria y semanal con bloques proporcionales al horario y duración, espacios libres y turnos superpuestos en columnas separadas. El mes mantiene el calendario por fechas con detalle del día. Incluye filtros, recurrencias y duplicación.
- Colores por cobro: verde para pagado completo, rojo para pendiente o pago parcial, azul para eventos personales. Bonificados y sin cargo en violeta, cancelados en gris.
- Reprogramación por arrastre en computadora o edición de fecha y hora en cualquier dispositivo.
- Fichas con historial de sesiones y pagos, honorarios, deuda y saldos a favor.
- Cobros parciales, asistencia, bonificaciones, cancelaciones y anulación de cobros.
- Gestor de gastos con categorías editables, colores, búsqueda y filtros por categoría y estado; gráficos por categoría, tramo del mes y año debajo de los movimientos.
- Patrimonio con activos, pasivos, patrimonio neto, historial de ajustes, evolución anual y copia de saldos anteriores sin reemplazar cuentas existentes.
- Buscador general, borradores para WhatsApp, navegación móvil y modo oscuro.
- Importación y respaldo JSON; informes CSV.
- Carga adicional de fichas y turnos mediante archivos privados, sin borrar registros existentes.
- Campos desconocidos vacíos y honorarios pendientes de completar.
- Días nacionales, provinciales y personales destacados en el calendario.
- Lectura privada de respuestas de Google Forms, con autorización de la cuenta propietaria.

## Primeros pasos

1. Abrí el enlace en Chrome o Safari desde el celular. También podés abrir el HTML descargado en un navegador moderno.
2. Creá un paciente y elegí su honorario y modalidad.
3. Agendá su sesión, o una serie con cantidad definida.
4. Registrá asistencia y cobro por separado. Se admiten pagos parciales.
5. Descargá respaldos JSON regularmente desde **Más**.

## Gastos y patrimonio

En **Economía → Movimientos**, elegí **Nuevo gasto** y completá concepto, importe, fecha, categoría, estado y medio de pago. Podés crear una categoría desde el formulario sin perder los campos escritos. En **Categorías y colores**, cambiá nombres y colores o archivá categorías; sus gastos anteriores se conservan.

Los totales y gráficos por categoría y tramo del mes distinguen los gastos pagados de los pendientes y planificados. Tocá una categoría del gráfico para filtrar sus movimientos. El gráfico anual compara ingresos registrados con gastos efectivamente pagados; tocá un mes para abrirlo. Los gráficos están en la misma pestaña: desplazate hacia abajo.

En **Patrimonio**, agregá activos y pasivos, abrí una cuenta para editar su saldo y consultar los ajustes, y usá **Traer saldos anteriores** para iniciar un nuevo período. Esa acción muestra los saldos antes de copiarlos y conserva las cuentas ya cargadas. El patrimonio neto es activos menos pasivos. Los pagos y gastos nuevos afectan la cuenta de su medio de pago; los gastos a pagar y planificados no descuentan dinero.

## Agenda por bloques

En **Semana**, las siete miniaturas permiten reconocer rápidamente días libres, mañanas y tardes ocupadas. Debajo, deslizá la grilla hacia los costados para recorrer los días y bajá para ver la tarde. Todos comparten la misma escala horaria. Los bloques tienen su duración real y los huecos quedan visibles; tocar un bloque abre el turno. Tocar un horario libre abre un turno con esa fecha y hora.

En **Mes**, se conserva el calendario por fechas. Cada día muestra su cantidad y un resumen con colores: pagados en verde, pendientes en rojo y personales en azul. Tocá la fecha o su resumen para consultar los nombres, horarios y estado de cobro debajo. Los feriados conservan sus colores y nombres. Los turnos cancelados no cuentan como tiempo ocupado.

El color del turno depende del cobro, separado de la asistencia y la modalidad: pasa a verde al registrar el pago completo. Si el pago es parcial queda rojo; anular un cobro devuelve el turno a rojo cuando corresponde. Los honorarios por completar también quedan rojos con una indicación específica. Los turnos bonificados o sin cargo se distinguen en violeta.

Al elegir **Nuevo turno**, desplegá **Qué querés agendar → Evento personal** para agregar médico, trámites u otras actividades. Completá título, fecha, hora y duración. El evento aparece en azul en las vistas de agenda y puede editarse, cancelarse o quitarse. Se controla que no se superponga con sesiones u otros eventos. No genera pacientes, honorarios, deudas ni cobros; se incluye en el respaldo completo.

## Cargar fichas y agenda sin borrar lo anterior

En **Más → Cargar fichas y agenda**, elegí un archivo privado de carga y revisá el resumen antes de **Agregar a Camicas**. La carga añade fichas y turnos, conserva cambios manuales y evita repetir los mismos registros. Los honorarios desconocidos no se tratan como sesiones gratuitas y no se pueden cobrar hasta completar su importe. No se deduce asistencia ni se inventan pagos.

Si el archivo incluye la configuración pública de conexión, prepara el acceso al formulario, pero el permiso para leer respuestas debe autorizarse en Google. Los archivos privados nunca se incluyen en el repositorio público.

## Fechas destacadas de octubre a diciembre de 2026

- 12 de octubre: Día del Respeto a la Diversidad Cultural.
- 9 de noviembre: feriado nacional por la visita del Papa León XIV.
- 10 de noviembre: feriado provincial de Córdoba por esa visita.
- 23 de noviembre: Día de la Soberanía Nacional, trasladado desde el 20.
- 7 de diciembre: día no laborable con fines turísticos, identificado como tal.
- 8 de diciembre: Inmaculada Concepción.
- 25 de diciembre: Navidad.

Se verificaron en la [Ley 27.399](https://www.argentina.gob.ar/normativa/nacional/ley-27399-281835/texto), el [Decreto 1103/2026](https://www.argentina.gob.ar/normativa/nacional/norma-430580/texto) y la [Resolución 164/2025](https://www.argentina.gob.ar/normativa/nacional/norma-421799/texto). Cada fecha permite consultar la norma. Las fechas personales son registros locales y se distinguen de los feriados legales.

## Migración

En el [sitio original](https://camicas-consultorio.sgonzalez372.chatgpt.site/), elegí **Más → Exportar copia completa**. En esta versión, elegí **Más → Importar una copia de Camicas**.

La importación valida referencias, identificadores, fechas e importes. Reemplaza el guardado local; no combina ni duplica copias. Conserva una copia recuperable y descarga el guardado anterior. Los saldos patrimoniales originales no se recalculan sumando de nuevo sus movimientos.

El formato se verificó con una copia original. Su tabla de gastos y ahorros estaba vacía: otros archivos deben superar la validación de esos registros. Los campos adicionales se conservan.

## Datos y límites

Los registros se guardan **en el navegador y dispositivo utilizados, sin contraseña propia de Camicas ni cifrado local**. No se envían a GitHub ni al servidor del sitio. GitHub almacena el código; no contiene la base de pacientes del consultorio.

La conexión opcional de Google Forms incorpora fichas nuevas y completa campos vacíos; conserva los cambios manuales. Necesita una configuración inicial y la autorización de Google en cada sesión. Consulta respuestas cada cinco minutos mientras la app está abierta, visible y autorizada; al vencer el permiso, hay que renovarlo con el botón. No funciona con la app cerrada.

No hay sincronización de agenda, pagos o cambios manuales entre dispositivos ni con el sistema original. Cambiar de navegador o dirección puede abrir un almacenamiento diferente: exportá e importá un respaldo para trasladar datos. Borrar los datos del navegador puede eliminar los registros.

No se trasladan la autenticación, los registros del servidor, la instalación PWA completa ni las notificaciones con la aplicación cerrada. Las series importadas conservan sus turnos existentes; no generan nuevas sesiones indefinidamente.

Los cobros nuevos actualizan la cuenta de su medio de pago. La edición de gastos e ingresos antiguos importados cambia la actividad, pero requiere revisar el saldo patrimonial por separado: la interfaz lo indica. Cancelar o bonificar conserva los cobros anteriores como saldo a favor, sin reasignarlos automáticamente.

## Publicación

El sitio se publica con GitHub Pages desde la rama `main`, carpeta raíz `/`. El repositorio público contiene únicamente el código, los íconos y las guías. Los registros administrativos permanecen en el navegador del dispositivo; no se suben con las actualizaciones del sitio.

## Verificación

Se probaron los formularios, navegación, agenda, pagos parciales, gastos, recurrencias, arrastre, superposiciones, importación y recuperación en una vista local. Se revisó el diseño en tamaños de computadora y celular. Las nuevas preferencias de bienvenida no modifican los datos administrativos.
