2 modelos normalmente GK420T, ZD420 y otras

[https://supportcommunity.zebra.com/s/article/ZD620-ZD420-Factory-Reset?language=es](https://supportcommunity.zebra.com/s/article/ZD620-ZD420-Factory-Reset?language=es)

Verificar conexión

- Ver que los cables estén bien conectados (USB o red).
- Si es red: abrir CMD en Windows y hacer ping a la IP de la impresora.
- Si no responde, puede estar apagada o fuera de red.
- Comprobar si el hostname funciona desde navegador (ej: [http://ZEBRA-123456](http://ZEBRA-123456)).

Sacar hoja de red

- ZD420: mantener presionado el botón “Feed” (flecha hacia abajo) al encender, soltar cuando parpadea 2 veces.
- GK420T: presionar los 2 botones de la izquierda al encender hasta que salga la hoja.
- Sirve para ver IP, modo de red, MAC y hostname.

Reiniciar rápido

- Apagar la impresora y volver a encender.
- También se puede desenchufar y volver a conectar.

Reiniciado de fábrica

- ZD420: mantener presionado el botón de Feed al encender hasta que parpadee 4 veces.
- Otra opción: abrir navegador, poner IP o hostname → ir a configuración → opción “Factory Default”.
- Esto borra configuraciones de red, papel, etc. Volver a configurar.

Vincular en computadora

- Entrar a “Dispositivos e impresoras” desde el panel de control de Windows.
- Si está como “Desconocida” o en gris: reinstalar.
- Si cambió de puerto USB, puede estar asignada a otro (USB001, USB002, etc.). Ver en pestaña “Puertos”.
- Debe figurar como “ZDesigner ZD420” o “Zebra GK420T”.

Desarmar y limpieza

- Apagar la impresora.
- Abrir la tapa y levantar el cabezal con el gancho lateral.
- Limpiar el cabezal con paño seco o alcohol isopropílico.
- Verificar que no haya etiquetas pegadas o trabadas.
- Revisar el sensor: debe estar centrado.

Significado de luces y botones

GK420T:

- Luz verde fija: lista.
- Luz roja fija: error (papel trabado, sin papel, tapa mal cerrada).
- Luz parpadeando rápido: en proceso de calibración o impresión.

Botón Feed:

- Un toque: avanza una etiqueta.
- Mantener al encender: calibración o imprimir hoja de red.

ZD420:

- Una sola luz LED con varios colores:

- Verde fija: OK.
- Naranja parpadeando: sin papel o error.
- Rojo fijo: error crítico (cabezal abierto, mal papel).
- Azul: comunicación por Bluetooth o modo especial.

Botón Feed:

- Un toque: avanza etiqueta.
- Mantener al encender:

- 2 parpadeos: hoja de red.
- 4 parpadeos: reset de fábrica.
- 5+: otros modos avanzados (no usar sin saber).

Problema: imprime en blanco

- Papel colocado del lado incorrecto (el lado térmico debe estar hacia arriba).
- Sensor mal ubicado → acomodar la flecha en el medio del rollo.
- Puede necesitar calibración: mantener botón Feed al encender hasta que parpadee 2 veces.
- Verificar si el tipo de papel es correcto (directo térmico sin ribbon en ZD420).

Problema: imprime cortado o fuera de margen

- Ver desde navegador (entrando por IP o hostname).
- Ir a “Settings” → “Print Width” → ancho: 834, alto: 3000.
- Guardar cambios.
- En Windows: ir a “Dispositivos e impresoras” → clic derecho en Zebra → Propiedades → Pestaña “Configuración” o “Preferencias” → Tamaño del papel: 10 x 15 cm.

Problema: no imprime tickets de calidad

- Verificar conexión.
- Asegurarse de que esté bien instalada en Windows.
- Ver si el sistema la reconoce como impresora válida.
- Probar hacer ticket desde otra PC o área para descartar problema de sistema.
- Puede ser necesario reinstalar o verificar puerto (en Propiedades > Puertos).

Problema: no detecta el papel

- Revisar que el papel no esté arrugado o mal cortado.
- Verificar que el sensor esté alineado al centro.
- Hacer calibración manual (Feed al encender).
- Revisar si el tipo de papel es compatible (térmico directo o con ribbon según modelo).
- Asegurarse de que las etiquetas estén dentro del rango de tamaño configurado.

Problema: etiquetas trabadas o se termina el rollo

- Apagar impresora.
- Abrir tapa.
- Sacar el rollo, quitar etiquetas trabadas.
- Revisar si el cabezal está limpio y libre de restos.
- Colocar un nuevo rollo con el sensor centrado.

Problema: el botón no responde o no hace nada

- Apagar y volver a encender.
- Revisar que la tapa esté bien cerrada.
- Si sigue sin funcionar, puede estar dañado el botón.
- En ese caso, intentar operar desde IP o cambiar la impresora.

Problema: cabezal dañado

- Imprime con líneas blancas o zonas vacías fijas.
- Aunque se cambie el papel, siempre falta parte de la impresión.
- Revisar con linterna si el cabezal está rayado o quemado.
- No se puede reparar, se cambia el cabezal o la impresora completa.

Acceso por IP o hostname (interfaz web)

- Poner en navegador la IP o nombre de red (ej: [http://ZEBRA-123456](http://ZEBRA-123456)).
- Desde ahí se puede:  
     Ver estado general.  
     Cambiar tamaño de papel (Settings > Print Width → 834 x 3000).  
     Resetear impresora a fábrica.  
     Ver temperatura del cabezal.  
     Ver logs de errores y último comando recibido.
- A veces pide usuario/contraseña: probar con “admin / 1234”.

Tamaño estándar de etiquetas en Windows

- Ir a: Dispositivos e impresoras > Zebra > Propiedades > Preferencias > Tamaño del papel.
- Seleccionar o crear tamaño 10 x 15 cm (corresponde a 834 x 3000 px).