# Camicas: acceso directo y respaldo

Camicas abre sin contraseña propia. Los pacientes, turnos y registros de economía se guardan en el navegador del celular y no se suben a GitHub. El guardado y los nuevos respaldos JSON no están cifrados por Camicas.

## Volver al acceso directo

1. Actualizá Camicas en el mismo acceso del celular que utilizás. Cerrá las otras pestañas de Camicas antes de recuperar registros.
2. Si no habías activado el cifrado, entrarás directamente.
3. Si aparece **Volver al acceso directo**, ingresá la contraseña anterior una sola vez y tocá **Recuperar mis registros**.
4. Revisá la cantidad de pacientes y turnos. Tocá **Recuperar y entrar sin contraseña**. Se recuperan los datos y se conserva el guardado cifrado anterior como respaldo.
5. Desde entonces, ese navegador abre sin pedir la contraseña ni bloquearse al salir.

Si el guardado cifrado estaba vacío y tenés los datos en otro archivo, podés elegir **Entrar y cargar mi JSON**. La copia cifrada anterior se conserva. En **Más**, elegí **Cargar fichas y agenda** para un archivo de carga, o **Importar una copia de Camicas** para un respaldo completo. Revisá siempre las cantidades antes de confirmar.

## Copias anteriores y nuevas

- Las copias que ya estaban cifradas siguen necesitando la contraseña anterior para abrirse. La actualización no cambia esos archivos ni recupera contraseñas olvidadas.
- Si necesitás revisar el guardado cifrado anterior de este navegador, usá **Más → Revisar copia cifrada anterior**. Verás las cantidades antes de aceptar una importación que reemplaza los registros actuales.
- Las nuevas copias descargadas desde **Más → Descargar copia completa** son JSON sin contraseña. Guardalas en un lugar privado.
- La app no sincroniza automáticamente agenda o economía entre celulares, navegadores o el acceso agregado a la pantalla de inicio. Conservá respaldos antes de cambiar de acceso, borrar datos del navegador o cambiar de teléfono.

## Celular y GitHub

Usá el código y Face ID del celular, mantenelo actualizado y evitá compartirlo desbloqueado con personas que no deban acceder a estos registros.

La cuenta GitHub controla el código de la app. Mantené su contraseña propia y la verificación en dos pasos; no cargues pacientes ni respaldos al repositorio. Esto no agrega un control de acceso a los registros del celular. GitHub Pages sirve el sitio público: poner el repositorio como privado no hace que el sitio sea privado automáticamente y puede afectar su publicación según el plan.

[Configurar verificación en dos pasos de GitHub](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/configuring-two-factor-authentication) · [Visibilidad de GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site).
