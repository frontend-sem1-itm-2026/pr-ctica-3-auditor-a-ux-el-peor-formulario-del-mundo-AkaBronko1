# Auditoría UX — "El peor formulario del mundo"

## 📊 Hallazgos

| # | Problema detectado | Categoría | Evidencia | ¿Por qué es un problema? |
|---|---|---|---|---|
| 1 | En celular, el formulario se ve diminuto y hay que hacer zoom para leer o tocar los campos | Responsive | Vista del formulario en pantalla móvil | El formulario no se adapta a la pantalla del celular. Todo aparece muy pequeño y serían dificiles de tocar con el dedo. |
| 2 | Las instrucciones de la contraseña son dificiles de leer | Accesibilidad | Texto claro debajo de los campos de contraseña | El texto que explica los requisitos de la contraseña es tan claro que se confunde con el fondo blanco. Un usuario no puede leerlo sin forzar la vista. |
| 3 | Al escribir en un campo, ya no sabes para qué era ese campo | Accesibilidad | Todos los campos del formulario | Los campos solo muestran texto de sugerencia dentro del input, que desaparece en cuanto empiezas a escribir. Si te distrae o cometes un error, ya no sabes qué dato ibas a poner ahí. |
| 4 | El campo de fecha no abre un calendario ni ayuda a escribir la fecha correctamente | Validación | Campo "Fecha de nacimiento" | El campo de fecha se comporta como un campo de texto normal. El usuario tiene que adivinar el formato exacto, y si se equivoca no recibe ningún aviso de que el dato esta mal. |
| 5 | El formulario se puede enviar completamente vacío sin ningún aviso | Validación | Botón "Guardar" al final del formulario | Ningún campo está marcado como obligatorio. Al hacer clic en Guardar sin rellenar nada, el formulario no dice nada. El usuario no sabe si su registro se completó o fallo. |
| 6 | Los botones "Guardar" y "Cancelar" se ven iguales | UX | Fila de botones al final del formulario | Ambos botones son del mismo color azul. El usuario no puede saber de un vistazo cual es cual, por lo que es facil equivocarse. |
| 7 | Hay un botón "Borrar todo" justo al lado del botón de envío y no pide confirmación | UX | Fila de botones al final del formulario | Un clic accidental en "Borrar todo" elimina toda la información ingresada sin preguntar "¿estás seguro?". Es muy fácil activarlo por error cuando se intenta hacer clic en "Guardar". |
| 8 | Cuando algo sale mal, el formulario solo dice "vuelve a intentarlo" sin explicar qué falló | UX | Nota al pie del formulario | El propio formulario avisa que si hay un error, no mostrará detalles. El usuario no sabe qué campo tiene el problema ni cómo solucionarlo, lo que genera frustración total y abandono. |
| 9 | Un solo campo pide a la vez la nacionalidad, la religión y el estado civil | Contenido | Campo "Nacionalidad, religión y estado civil" | Es confuso meter tres datos tan distintos en un solo espacio. El usuario no sabe si separarlos con coma, barra u otro símbolo. Además, que te pidan la religión en un registro genérico resulta invasivo. |
| 10 | El título del formulario no dice para qué sirve este trámite | Jerarquía visual / Contenido | Encabezado principal del formulario | El titulo "Formulario General Universal de Registro, Inscripción, Solicitud y Validación Inicial" es tan largo y vago que el usuario no sabe si está registrándose, haciendo una solicitud o iniciando un tramite. |
| 11 | En pantalla grande, el formulario queda en una franja estrecha y obliga a bajar mucho | Jerarquía visual / Layout | Vista de escritorio del formulario | En pantallas amplias el formulario ocupa solo la mitad izquierda de la pantalla. Hay mucho espacio desaprovechado y el usuario tiene que hacer scroll excesivo para llegar al botón de envío. |
| 12 | Los requisitos de la contraseña incluyen cosas imposibles como "jeroglíficos" y "buena vibra" | Contenido | Instrucciones bajo los campos de contraseña | Entre los requisitos aparecen "jeroglíficos" y "buena vibra". El usuario no sabe si es un error o un chiste, y en cualquier caso no puede cumplir esos requisitos. Genera desconfianza en toda la plataforma. |

---

## 📸 Evidencia visual

*(Ver archivos adjuntos en el repositorio)*

- `captura-escritorio.png` — Vista del formulario en navegador de escritorio.
- `captura-movil.png` — Vista del formulario en modo responsive/móvil.

---

En este archivo debes **listar los problemas encontrados** en el formulario.

Se recomienda clasificar los hallazgos usando las siguientes categorías:

### Categorías sugeridas

**UX (Experiencia de usuario)**  
- claridad del flujo  
- botones confusos  
- acciones poco claras  

**Accesibilidad**  
- falta de labels  
- bajo contraste  
- problemas de navegación  

**Validación**  
- campos sin validación  
- tipos incorrectos  
- campos que deberían ser `required`  

**Jerarquía visual / Layout**  
- orden incorrecto  
- agrupación deficiente  
- mala organización de campos  

**Responsive**  
- problemas en pantalla móvil  
- layout que se rompe  
- elementos demasiado grandes o pequeños  

**Contenido**  
- textos confusos  
- requisitos absurdos  
- instrucciones poco claras  

---

# 📊 Formato recomendado

Puedes usar una tabla como esta:

| # | Problema detectado | Categoría | Evidencia | ¿Por qué es un problema? |
|---|---|---|---|---|
| 1 | El campo nombre no tiene label | Accesibilidad | Campo “Nombre” | Los lectores de pantalla no pueden interpretarlo correctamente |
| 2 | Botón cancelar junto al enviar | UX | Botones al final | Puede provocar errores al usuario |
| 3 | Confirmar correo es opcional | Validación | Campo email | Puede causar inconsistencias |

Se recomienda identificar **al menos 10 problemas**.

---

# 📸 Evidencia visual

Además del archivo `AUDITORIA.md`, debes agregar **capturas de pantalla** del formulario.

Incluye al menos:

### 1️⃣ Vista en escritorio
Ventana normal del navegador.

### 2️⃣ Vista en móvil
Ventana reducida o modo responsive del navegador.

Puedes nombrarlas por ejemplo:
captura-escritorio.png
captura-movil.png

---
# 🚫 Regla importante

❌ **No debes modificar el HTML o CSS del formulario.**  

Esta actividad es únicamente de **análisis y auditoría**.
---

# 📦 Entrega

Realiza un **commit en tu repositorio** que incluya:

AUDITORIA.md
captura-escritorio.png
captura-movil.png


Mensaje de commit sugerido:
Auditoría UX del formulario: identificación de problemas de diseño


---

# 💡 Consejo

Piensa como un **usuario real** que intenta completar el formulario.

Si algo te confunde, probablemente **también confundirá a otros usuarios**.
