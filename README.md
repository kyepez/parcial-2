Este código forma un **pequeño sitio web completo de adopción de mascotas** llamado **Patitas Felices**, 100% funcional solo con HTML, CSS y JavaScript (sin servidor ni base de datos). Está compuesto por **3 páginas** que trabajan juntas usando `localStorage` del navegador.

### Resumen general del proyecto

| Página         | Nombre del archivo | Qué hace                                                                 |
|----------------|--------------------|---------------------------------------------------------------------------|
| 1              | `login.html`       | Página de inicio / login                                                  |
| 2              | `catalogo.html`    | Catálogo de mascotas disponibles para adoptar                             |
| 3              | `carrito.html`     | Lista de “Mis Mascotas Favoritas” (las que marcaste para adoptar)         |

Todo funciona en tu navegador, incluso sin internet (una vez cargadas las imágenes).

### Funcionamiento paso a paso

1. **Abres `login.html` (o `index.html` si lo renombraste)**  
   - Es una pantalla bonita con fondo degradado verde.  
   - Pides tu nombre y cualquier contraseña (no valida nada, solo que no estén vacíos).  
   - Al hacer clic en “Ingresar”:  
     → Guarda en el navegador:  
     ```js
     localStorage.setItem('loggedIn', 'true');
     localStorage.setItem('username', 'el nombre que escribiste');
     ```  
     → Te redirige automáticamente a `catalogo.html`

2. **Llegas a `catalogo.html`**  
   - Si no estás logueado → te manda de vuelta al login.  
   - Te saluda por tu nombre: “¡Hola, Ana!”  
   - Muestra un contador de corazones (al lado del saludo).  
   - Aparecen 6 tarjetas muy bonitas con fotos de mascotas (Luna, Max, Canela, etc.).  
   - Cada tarjeta tiene un botón naranja “¡Quiero adoptarlo!”  
   - Al hacer clic en el botón:  
     → Se guarda el nombre de la mascota en una lista de favoritos  
     → Se actualiza el contador de corazones  
     → Sale un mensaje: “Te contactaremos pronto”

3. **Vas a `carrito.html` (puedes poner un enlace desde el catálogo o escribir la URL directamente)**  
   - También verifica que estés logueado.  
   - Muestra la lista de todas las mascotas que marcaste como favoritas.  
   - Cada una tiene un botón rojo “✕” para quitarla de la lista.  
   - Si no tienes ninguna → muestra un mensaje triste: “Aún no has elegido ninguna mascota”.  
   - Botón para “Volver al catálogo”.

### Características técnicas y de diseño

- Diseño muy bonito y moderno (colores verdes, tarjetas con sombra y hover, botones redondeados)
- Totalmente responsive (se ve bien en móvil y escritorio)
- Usa Google Fonts (Poppins)
- Todo se guarda en el navegador del usuario (`localStorage`) → los favoritos persisten aunque cierres y abras de nuevo
- No hay backend ni base de datos → perfecto para proyectos escolares, portafolios o prototipos

### En resumen: ¿Qué hace este código?

Es una **aplicación web completa y adorable de adopción de mascotas** donde:

1. Te registras con tu nombre  
2. Ves mascotas hermosas en adopción  
3. Eliges las que te gustan (como un “carrito de adopción”)  
4. Ves y gestionas tu lista de mascotas favoritas  
5. Todo queda guardado en tu navegador

Un proyecto ideal para aprender:
- HTML + CSS moderno (Flexbox, Grid, sombras, transiciones)
- JavaScript básico-intermedio
- localStorage
- Navegación entre páginas
- Experiencia de usuario (UX) bonita y amigable

¡Es un excelente ejemplo de mini-app educativa y muy bien hecha!  
Si lo subes a GitHub Pages o Netlify, cualquiera puede usarlo en segundos.
