# Amigo Secreto

Descripción del Proyecto

**Amigo Secreto** es una aplicación web interactiva que permite a los usuarios organizar un sorteo de "Amigo Secreto" de manera sencilla. Los usuarios pueden agregar nombres de amigos a una lista mediante un campo de texto y un botón. Luego, al realizar el sorteo, la aplicación selecciona un nombre al azar y lo muestra en pantalla. El proyecto está desarrollado con HTML, CSS y JavaScript, utilizando un diseño responsivo y accesible.

Funcionalidades

- **Agregar nombres**: Los usuarios pueden ingresar nombres en un campo de texto y añadirlos a una lista visible con el botón "Añadir".
- **Validación de entrada**: Si el campo de texto está vacío, se muestra una alerta solicitando un nombre válido.
- **Visualización de la lista**: Los nombres ingresados se muestran en una lista ordenada en la página.
- **Sorteo aleatorio**: Al hacer clic en el botón "Sortear Amigo", se selecciona un nombre al azar de la lista y se muestra como el "Amigo Secreto".
- **Interfaz amigable**: Incluye estilos modernos con fuentes de Google Fonts y un diseño claro.

Requisitos

- Un navegador web moderno (Chrome, Firefox, Edge, etc.).
- Un editor de código como Visual Studio Code (opcional, para modificar el proyecto).
- Conexión a internet para cargar las fuentes de Google Fonts (opcional si las fuentes se alojan localmente).

Instrucciones de Uso

1. Ingresa el nombre de un amigo en el campo de texto proporcionado.
2. Haz clic en el botón **Añadir** para agregar el nombre a la lista.
3. Repite el proceso para añadir más nombres (mínimo 1 nombre para realizar el sorteo).
4. Haz clic en el botón **Sortear Amigo** para seleccionar un nombre al azar.
5. El resultado del sorteo aparecerá en pantalla, indicando quién es el "Amigo Secreto".

Cómo Ejecutar el Proyecto

### 2. Estructura del Proyecto

Asegúrate de que la estructura de archivos sea la siguiente:

```
amigo-secreto/
├── assets/
│   ├── amigo-secreto.png
│   ├── play_circle_outline.png
├── index.html
├── style.css
├── app.js
└── README.md
```

### 3. Abrir la Aplicación

- **Opción 1**: Abre el archivo `index.html` directamente en un navegador web haciendo doble clic sobre él.
- **Opción 2**: Usa un servidor local para evitar problemas con recursos locales:
  - Si usas Visual Studio Code, instala la extensión **Live Server** y ejecuta el proyecto.
  
## Posibles Problemas y Soluciones

1. **El sorteo muestra "undefined" o no funciona**:

   - **Causa**: El archivo `app.js` no está correctamente vinculado o el DOM no está cargado.
   - **Solución**: Asegúrate de que el archivo `app.js` esté en la misma carpeta que `index.html` y que el tag `<script src="app.js" defer></script>` incluya el atributo `defer`.

2. **Las imágenes no se muestran**:

   - **Causa**: Las imágenes en la carpeta `assets/` no están en la ruta correcta.
   - **Solución**: Verifica que los archivos `amigo-secreto.png` y `play_circle_outline.png` estén en la carpeta `assets/` y que las rutas en `index.html` sean correctas.

3. **El botón "Añadir" o "Sortear Amigo" no responde**:

   - **Causa**: Puede haber un error en el JavaScript o un problema con los eventos.
   - **Solución**: Abre la consola del navegador (F12 &gt; Consola) y verifica si hay errores. Asegúrate de que las funciones `agregarAmigo()` y `sortearAmigo()` estén definidas en `app.js`.

## Tecnologías Utilizadas

- **HTML5**: Estructura de la página.
- **CSS3**: Estilos y diseño responsivo.
- **JavaScript**: Lógica para agregar nombres, validar entradas y realizar el sorteo aleatorio.

## Contribuciones

¡Las contribuciones son bienvenidas! Si deseas mejorar el proyecto:

1. Haz un fork del repositorio.
2. Crea una rama para tu funcionalidad (`git checkout -b feature/nueva-funcionalidad`).
3. Realiza tus cambios y haz commit (`git commit -m "Añadir nueva funcionalidad"`).
4. Sube los cambios a tu fork (`git push origin feature/nueva-funcionalidad`).
5. Abre un Pull Request en GitHub.

