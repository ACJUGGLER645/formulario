# Formulario

Este proyecto es un ejemplo práctico de cómo crear un formulario sencillo en una página web utilizando **HTML, CSS y JavaScript**. Permite al usuario ingresar su nombre, apellido, celular y correo electrónico, mostrando una ventana de confirmación con los datos capturados.

---

## ¿Qué hace este proyecto?

* Presenta un formulario con campos básicos de texto, número y correo.
* Valida que todos los campos estén llenos antes de enviar.
* Muestra los datos ingresados en un cuadro de confirmación.
* Recarga la página después de la confirmación.

---

## ¿Con qué está hecho?

* **HTML**: estructura el formulario y define los campos de entrada.
* **CSS**: le da estilo al formulario para que sea más legible y estético.
* **JavaScript**: controla lo que sucede cuando se envía el formulario.

---

## Archivos principales

* `index.html`: contiene el formulario y los campos de entrada.
* `style.css`: define la apariencia del formulario.
* `script.js`: controla la interacción al enviar los datos.

---

## Explicación de las funciones utilizadas

En el archivo **script.js** se manejan las siguientes funciones y métodos:

1. **`document.getElementById()`**

   * Obtiene elementos de la página por su identificador (`id`).
   * Ejemplo:

     ```js
     let nombre = document.getElementById("nombre").value;
     ```

2. **`addEventListener("submit", ...)`**

   * Escucha cuando se envía el formulario.
   * Permite ejecutar código personalizado en lugar de enviar directamente los datos.

3. **`e.preventDefault()`**

   * Evita que el formulario recargue la página automáticamente al ser enviado.
   * Esto da tiempo para validar o mostrar mensajes al usuario.

4. **`confirm()`**

   * Muestra una ventana emergente con un mensaje y dos opciones: **Aceptar** o **Cancelar**.
   * Se utiliza para preguntar al usuario si los datos mostrados son correctos.
   * Ejemplo:

     ```js
     confirm("¿Los datos son correctos?");
     ```

5. **`location.reload()`**

   * Recarga la página actual.
   * En este proyecto se usa después de la confirmación.

---

## Posibles mejoras

* Guardar los datos en el almacenamiento local o en una base de datos.
* Mostrar los datos confirmados en la misma página en lugar de un `confirm()`.
* Cambiar el recargado de página por un mensaje de éxito.

---

**Autor:** Jhon Alejandro Correal Martinez  
**Asignatura:** Programación III  
**Programa:** Tecnología en Desarrollo de Software – Facultad de Sistemas  
**Institución:** Escuela Tecnológica Instituto Técnico Central 


