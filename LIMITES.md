# Límites de la aplicación

## Acceso libre
La aplicación no tiene usuarios ni contraseñas. Cualquiera que abra la dirección puede ver y cambiar todas las actividades. Es un panel personal, no una aplicación segura.

## Reglas solo en el navegador
Las reglas del título (mínimo 3 caracteres, sin repetidos) se validan en el navegador. Si alguien envía una petición directa al servidor, por ejemplo con `curl`, se las salta. Sirven para ayudar a quien escribe, no para proteger los datos.

## localStorage
Los datos ya no se guardan en `localStorage`. Si volviera, no está cifrado y cualquier script de la página puede leerlo.

## Cosas que vi y no arreglé
- No hay prueba de `alternarDestacada`.
- `formulario-actividad` pesa 65 kB, bastante más que las otras páginas diferidas.  