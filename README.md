# Camicas · Consultorio

Agenda, pacientes y economía para un consultorio individual. Versión violeta, con detalles florales discretos y mensajes de bienvenida opcionales.

**Abrir desde el celular:** https://camicas59.github.io/camicas-consultorio/

El diseño prioriza el uso táctil: navegación inferior, formularios de una columna, controles cómodos, márgenes para la zona segura del teléfono y gráfico anual distribuido en cuatro columnas. Se verificó desde 320 píxeles de ancho.

## Archivos

- `index.html`: aplicación completa como página inicial.
- `camicas-v2.html`: la misma aplicación en un archivo HTML independiente.
- `.nojekyll`: sirve el HTML como sitio estático sin procesamiento adicional.
- `.gitignore`: excluye respaldos, CSV y archivos locales de trabajo.

Los dos HTML son idénticos. El uso local no requiere compilación ni paquetes. La conexión opcional con Google Forms requiere internet y autorización de Google. El código no contiene pacientes reales ni registros de prueba.

## Apariencia y bienvenida

La paleta combina violeta suave y lavanda. El modo oscuro mantiene esa familia de colores. Las flores acompañan los controles habituales; no hay botón de pausa ni temporizadores.

Al abrirse o volver a la aplicación, puede aparecer una bienvenida encima de la pantalla. Hay que cerrarla con la X o **Entrar a Camicas**. Se muestra como máximo dos veces por día y con al menos seis horas entre mensajes; no queda como una tarjeta del inicio. El cartel muestra la cita y su autor, con la X y **Entrar a Camicas** como únicas acciones. El límite se cuenta en el navegador del celular. La preferencia general se administra desde **Más**.

Las citas se verificaron en fuentes de sus autores o de sus comunidades editoras. Las citas originalmente en inglés se presentan en español. Sus fuentes se conservan aquí; el cartel muestra solamente el autor:

- [Kristin Neff · Self-Compassion](https://self-compassion.org/).
- [Tara Brach · Judgment, Acceptance and Freedom](https://www.tarabrach.com/judgment-acceptance-freedom-retreat/).
- [Thich Nhat Hanh · Calming the Breath Gatha, Plum Village](https://web.plumvillage.app/item/calming-the-breath-gatha).
- [Thich Nhat Hanh · Teachings on True Transmission, Plum Village](https://plumvillage.org/articles/teachings-on-true-transmission).

## Funciones

- Inicio con próximos turnos, indicadores, cobros y recordatorios administrativos.
- Agenda diaria, semanal, mensual y de próximos turnos; filtros, recurrencias y duplicación.
- Reprogramación por arrastre en computadora o edición de fecha y hora en cualquier dispositivo.
- Fichas con historial de sesiones y pagos, honorarios, deuda y saldos a favor.
- Cobros parciales, asistencia, bonificaciones, cancelaciones y anulación de cobros.
- Economía con gráfico anual, gastos, otros ingresos, activos, pasivos, ahorros y traspasos.
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

Los registros se guardan **en el navegador y dispositivo utilizados**, sin contraseña ni cifrado. No se envían a GitHub ni al servidor del sitio. GitHub almacena el código; no contiene la base de pacientes del consultorio.

La conexión opcional de Google Forms incorpora fichas nuevas y completa campos vacíos; conserva los cambios manuales. Necesita una configuración inicial y la autorización de Google en cada sesión. Consulta respuestas cada cinco minutos mientras la app está abierta, visible y autorizada; al vencer el permiso, hay que renovarlo con el botón. No funciona con la app cerrada.

No hay sincronización de agenda, pagos o cambios manuales entre dispositivos ni con el sistema original. Cambiar de navegador o dirección puede abrir un almacenamiento diferente: exportá e importá un respaldo para trasladar datos. Borrar los datos del navegador puede eliminar los registros.

No se trasladan la autenticación, los registros del servidor, la instalación PWA completa ni las notificaciones con la aplicación cerrada. Las series importadas conservan sus turnos existentes; no generan nuevas sesiones indefinidamente.

Los cobros nuevos actualizan la cuenta de su medio de pago. La edición de gastos e ingresos antiguos importados cambia la actividad, pero requiere revisar el saldo patrimonial por separado: la interfaz lo indica. Cancelar o bonificar conserva los cobros anteriores como saldo a favor, sin reasignarlos automáticamente.

## Publicación

El sitio se publica con GitHub Pages desde la rama `main`, carpeta raíz `/`. El repositorio público contiene únicamente el código y esta guía. Los registros administrativos permanecen en el navegador del dispositivo; no se suben con las actualizaciones del sitio.

## Verificación

Se probaron los formularios, navegación, agenda, pagos parciales, gastos, recurrencias, arrastre, superposiciones, importación y recuperación en una vista local. Se revisó el diseño en tamaños de computadora y celular. Las nuevas preferencias de bienvenida no modifican los datos administrativos.
