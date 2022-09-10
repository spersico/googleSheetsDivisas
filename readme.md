# Divisas (Argentina) en Google Sheets
Script para obtener los valores actuales de las divisas (Dolar y Euro), en los mercados **oficial** y **blue**, en una hoja de cálculo de Google Sheets.

Super útil para llevar tus finanzas personales en Argentina!.

Basado en [este script](https://github.com/qeet/IMPORTJSONAPI) genial de [@qeet](https://github.com/qeet), y la genial API de [Bluelytics](https://bluelytics.com.ar/#!/)

![msedge_GxRq5TX0qe](https://user-images.githubusercontent.com/10502605/189499875-d8bb767e-2aa8-4185-8549-3bfb8b5fbc37.png)
###  Instalación
Para instalar esta función custom en una hoja de cálculo de Google Sheets, seguí los siguientes pasos:

1. Abrí la hoja de cálculo en un navegador.
2. Andá al menú Extensiones, item AppScript:

![msedge_XK1h0RwqQ1](https://user-images.githubusercontent.com/10502605/189499907-ce0d5c83-fdc7-447b-b7e1-fbad2e1d2500.png)

Esto va a abrir un editor en una pestaña nueva, con un archivo llamado Código.gs, en un proyecto llamado Proyecto sin Título.

3. Vas a tener que copiar y pegar el contenido de [este archivo](https://raw.githubusercontent.com/spersico/googleSheetsDivisas/main/codigo.gs), reemplazando todo lo que tenga inicialmente el archivo Código.gs
4. Ahora podés guardar el script haciendo click en el botón Guardar Proyecto.
![msedge_BXn3A0C2aT](https://user-images.githubusercontent.com/10502605/189499922-46357d08-c610-49a7-9926-fd4a43995c94.png)

5. Listo! Ahora podés cerrar la pestaña del editor, y podés continuar en tu hoja de cálculo.
6. En la hoja de cálculo, podés usar en cualquier lado alguna de estas funciones (ninguna lleva parametros):
 - `COTIZACION_DOLAR_BLUE`
 - `COTIZACION_EURO_BLUE`
 - `COTIZACION_DOLAR_OFICIAL`
 - `COTIZACION_EURO_OFICIAL`
 
Acá podés ver un ejemplo de una función andando:

![msedge_hwm66UePPh](https://user-images.githubusercontent.com/10502605/189499925-14ce8469-3846-4b5a-84b6-373d339116bd.png)

### Preguntas Frecuentes (FAQ)

- **Tengo que hacer esto en una hoja de calculo nueva, o puedo usar lo que ya tengo?**
    - No, no hace falta hacer una hoja de cálculo nueva. Podés agregarle este script a cualquier hoja de cálculo.
   
- **Ya seguí todos los pasos, no me carga!. Que hago?**

   - En algunas ocasiones puede que no cargue los valores. Esto puede darse por dos razones:
        + Google Sheets se traba un poco a veces **(probá recargando la página)**.
        + La API de Bluelytics está caída o está sobrecargada. A tener en cuenta que esta API es gratuita y no tiene límites de uso, por lo que puede que esté caida o algo así. (Si la API no anda, toca esperar, probá recargando en una hora). 
          
          Podés verificar si la API funciona accediendo a la URL que este script usa: https://api.bluelytics.com.ar/v2/latest.
        
- **De donde salen los datos?**
    - Los datos salen de [Bluelytics](https://bluelytics.com.ar/#!), específicamente de [este endpoint](https://api.bluelytics.com.ar/v2/latest). Creo que esa API scrapea resultados de varios diarios (Ámbito, Cronista, La Nacion, y del BCRA) diariamente.

### Licencia y Soporte
[MIT](https://github.com/spersico/googleSheetsDivisas/blob/main/LICENSE).

Yo no tengo NADA que ver ni con [@qeet](https://github.com/qeet), ni con [Bluelytics](https://bluelytics.com.ar/#!/), estoy compartiendo esta modificación de mi script porque quería ver como era jugar con código de Google Sheets y me servía el script. Si se rompe, hacé un Issue o un PR y lo vemos, dale, pero no esperes mucho 😛.
