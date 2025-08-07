

Modelos comunes: MS321, MS421, MX310, MX611, etc.

---

### Como revisar conexión

**Por cable de red (Ethernet):**

- Verificar que el cable esté bien conectado y que la luz de red esté encendida (detrás de la impresora, cerca del puerto).
    
- En el panel de la impresora, ir a **Menú > Configuración de red > Dirección IP** para ver si tiene asignada una IP.
    
- Desde una PC, abrir CMD y escribir:
    
    nginx
    
    CopiarEditar
    
    `ping IP_DE_LA_IMPRESORA`
    
    Si responde, está conectada.
    

**Por USB:**

- Ver en “Dispositivos e impresoras” si aparece con nombre “Lexmark”.
    
- Si no aparece o está en gris: reinstalar driver.
    

---

### Como calibrar

La mayoría de las impresoras Lexmark **no requieren calibración manual**.  
Si las impresiones salen mal alineadas o cortadas:

- En el panel, ir a **Menú > Configuración de bandeja > Tamaño del papel** y verificar que coincida con el tamaño cargado.
    
- También se puede ir a **Menú > Diagnóstico > Página de prueba** para verificar si hay errores.
    

---

### Como saber la IP

Método 1 – Desde el panel:

- Ir a **Menú > Información de red > Dirección TCP/IP**
    
- Otras rutas posibles: **Menú > Configuración de red > Ver dirección IP**
    

Método 2 – Imprimir hoja de configuración:

- Ir al menú y buscar **“Imprimir configuración”** o **“Página de red”**.
    
- O en algunos modelos:  
    **Menú > Informes > Página de configuración > Imprimir**
    

Método 3 – Por DHCP:

- Ver en el router o pedir a IT la IP asignada al hostname “Lexmark-XXXXX”.
    

---

### Como configurar

Desde el panel de la impresora:

- **Menú > Configuración de red**: para IP fija, DHCP, máscara de subred y puerta de enlace.
    
- **Menú > Configuración de bandejas**: para tamaño de papel (ej. A4, Carta).
    
- **Menú > Calidad de impresión**: ajustar intensidad, ahorro de tóner, etc.
    
- Guardar todos los cambios con “Aceptar” o “Aplicar”.
    

---

### Como entrar al panel interno (desde navegador)

1. Desde una PC, abrir el navegador.
    
2. Escribir la dirección IP de la impresora en la barra (ejemplo: `http://192.168.0.105`)
    
3. Aparece la **interfaz web de Lexmark**. Desde ahí podés:  
     - Ver estado de la impresora.  
     - Configurar red, idioma, calidad de impresión, papel, etc.  
     - Cambiar IP a fija (Menú Red > TCP/IP > Dirección manual).  
     - Reiniciar o resetear desde la web.  
     - Ver los trabajos en cola o errores.
    

Usuario y contraseña por defecto si lo pide:

yaml

CopiarEditar

`admin / 0000`

o

pgsql

CopiarEditar

`admin / admin`

---

### Como verificar si es problema de impresión

1. Imprimir una hoja de prueba:  
     - Ir a **Menú > Informes > Página de prueba o Configuración > Imprimir**  
     - Si imprime bien, el problema es del sistema o red, no de la impresora.
    
2. Probar imprimir desde otra computadora:  
     - Ir a Word, Bloc de notas u otro programa.  
     - Seleccionar la impresora Lexmark y mandar a imprimir.  
     - Si imprime, el problema es del sistema de calidad.
    
3. Ver si hay errores en el panel:  
     - Mensajes como “Papel atascado”, “Bandeja vacía”, “Sin tóner”, etc.
    

---

### Como instalar impresora en computadora

**Con cable USB:**

1. Conectar la impresora encendida al puerto USB.
    
2. Windows debería instalarla automáticamente.
    
3. Si no aparece, ir a **Panel de control > Dispositivos e impresoras > Agregar impresora > USB**.
    
4. Elegir “Lexmark” y el modelo correspondiente.
    

**Por red (IP fija):**

1. Ir a **Panel de control > Dispositivos e impresoras > Agregar impresora > La impresora no está en la lista**.
    
2. Elegir “Agregar por dirección TCP/IP”.
    
3. Escribir la IP de la impresora.
    
4. Elegir driver Lexmark o instalar desde archivo .inf (descargado de lexmark.com).
    
5. Finalizar. La impresora quedará instalada como red.
    

---

### Otras cosas importantes a saber:

- **Tamaño de papel**: generalmente A4 (210 x 297 mm).
    
- **Bandeja 1** es la más usada. Ver que tenga papel cargado correctamente.
    
- Si las hojas salen mal o cortadas, revisar configuración del papel tanto en el panel como en Windows.
    
- Si imprime lento o mal, reiniciar impresora desde el menú o desenchufar 10 segundos y volver a encender.
    
- Verificar si hay mensaje de tóner bajo o tambor agotado. En algunos modelos, pueden bloquear la impresión si no se resetean.