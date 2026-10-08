# Camicas · Consultorio

Agenda, pacientes y economía para un consultorio individual. Versión violeta, con detalles florales discretos y mensajes de bienvenida opcionales.

## Archivos

- `index.html`: aplicación completa como página inicial.
- `camicas-v2.html`: la misma aplicación en un archivo HTML independiente.
- `.nojekyll`: sirve el HTML como sitio estático sin procesamiento adicional.
- `.gitignore`: excluye respaldos, CSV y archivos locales de trabajo.

Los dos HTML son idénticos. No requieren compilación, paquetes ni servicios externos. El código no contiene pacientes reales ni registros de prueba.

## Apariencia y bienvenida

La paleta combina violeta suave y lavanda. El modo oscuro mantiene esa familia de colores. Las flores acompañan los controles habituales; no hay botón de pausa ni temporizadores.

Al abrirse, la aplicación puede mostrar una cita breve sin bloquear la agenda. Aparece la primera vez y después sólo ocasionalmente, como máximo una vez cada 18 horas. Se cierra con la X, se desactiva con **No mostrar más** y se reactiva desde **Más**.

Las citas se verificaron en fuentes de sus autores o de sus comunidades editoras. Son traducciones propias del inglés, y cada mensaje enlaza su fuente:

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

## Primeros pasos

1. Abrí el HTML en un navegador moderno. No uses una previsualización que desactive JavaScript.
2. Creá un paciente y elegí su honorario y modalidad.
3. Agendá su sesión, o una serie con cantidad definida.
4. Registrá asistencia y cobro por separado. Se admiten pagos parciales.
5. Descargá respaldos JSON regularmente desde **Más**.

## Migración

En el [sitio original](https://camicas-consultorio.sgonzalez372.chatgpt.site/), elegí **Más → Exportar copia completa**. En esta versión, elegí **Más → Importar una copia de Camicas**.

La importación valida referencias, identificadores, fechas e importes. Reemplaza el guardado local; no combina ni duplica copias. Conserva una copia recuperable y descarga el guardado anterior. Los saldos patrimoniales originales no se recalculan sumando de nuevo sus movimientos.

El formato se verificó con una copia original. Su tabla de gastos y ahorros estaba vacía: otros archivos deben superar la validación de esos registros. Los campos adicionales se conservan.

## Datos y límites

Los registros se guardan **en el navegador y dispositivo utilizados**, sin contraseña ni cifrado. No se envían a GitHub ni al servidor del sitio. GitHub almacena el código; no contiene la base de pacientes del consultorio.

No hay sincronización con el sistema original ni entre dispositivos. Cambiar de navegador o dirección puede abrir un almacenamiento diferente: exportá e importá un respaldo para trasladar datos. Borrar los datos del navegador puede eliminar los registros.

No se trasladan la autenticación, los registros del servidor, la instalación PWA completa ni las notificaciones con la aplicación cerrada. Las series importadas conservan sus turnos existentes; no generan nuevas sesiones indefinidamente.

Los cobros nuevos actualizan la cuenta de su medio de pago. La edición de gastos e ingresos antiguos importados cambia la actividad, pero requiere revisar el saldo patrimonial por separado: la interfaz lo indica. Cancelar o bonificar conserva los cobros anteriores como saldo a favor, sin reasignarlos automáticamente.

## Publicación

El repositorio contiene la página inicial lista para alojar como sitio estático. Crear el repositorio y cargar los archivos no publica automáticamente una dirección de la aplicación. La publicación requiere configurar un servicio de alojamiento por separado.

## Verificación

Se probaron los formularios, navegación, agenda, pagos parciales, gastos, recurrencias, arrastre, superposiciones, importación y recuperación en una vista local. Se revisó el diseño en tamaños de computadora y celular. Las nuevas preferencias de bienvenida no modifican los datos administrativos.
