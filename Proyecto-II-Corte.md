# Lineamientos

- Realizar la entrega en la fecha y hora correspondiente
- Entregar el software en un archivo con extensión **.c** y subirlo a su repositorio correspondiente.
- El software debe compilar sin errores.

# Proyecto

La empresa X Web Services requiere de un software para ordenar y listar las IPs por segmentos de red en cada uno de sus Data Centers. Para ello el software debe leer de un archivo pregenerado las IPs, asignarlas un Data Center  y poder listarlos. El resultado final debe ser otro archivo generado por el software con las IPs propiamente distribuidas.
El software debe tener en cuenta que el archivo pregenerado con las IPs proviene de un sistema Global de la empresa  y este puede ser dinámico, es decir, puede tener más o menos IPs dependiendo de la actividad de los clientes que contraten sus servicios, sin embargo, los segmentos de red permanecerán iguales.

## Ejemplo

**Archivo pregenerado: global_ip.txt**

| IPs | 
| -----------|  
| 172.120.160.1 |   
| 162.130.150.10 |
| 172.120.160.5|
| 162.130.150.43 |
| 173.150.10.10|

**Resultado:  ip_datacenter.txt**

 | US-California| AU-Sidney | VE-Caracas|
 |----------------|-----------------|------|
 |172.120.160.1 | 162.130.150.10 | 173.150.10.10|
 |172.120.160.5 | 162.130.150.43 | |
 
 **En la próxima generación del archivo pregenerado: global_ip.txt** 
 
 | IPs | 
| -----------|  
| 172.120.160.1 |   
| 162.130.150.10 |
| 172.120.160.5|
| 162.130.150.43 |
| 173.150.10.10|
| 173.150.10.11|

**Resultado:  ip_datacenter.txt** 

 | US-California| AU-Sidney | VE-Caracas|
 |----------------|-----------------|------|
 |172.120.160.1 | 162.130.150.10 | 173.150.10.10|
 |172.120.160.5 | 162.130.150.43 | 173.150.10.11|
 
## Evaluación

**Utilizar los data Centers mostrados en el ejemplo**

- Lectura del archivo pregenerado y escritura de archivo con la data ordenada - 3 pts
- Manejo de la data con las estructuras correspondientes - 3 pts
- Software funcional según lo requerido - 4 pts
