# Ejercicio T7.2: Sistemas ficheros en red
## Autor: Antonio Jesús Heredia Castillo
### Buscar información sobre los sistemas de ficheros en red más utilizados en la actualidad y comparar sus  características. Hacer una lista de ventajas e inconvenientes de todos ellos, así como grandes sistemas en los que se utilicen.

Los sistemas de ficheros en red son mecanismos para almacenar archivos en una red.  Permite a los usuarios acceder a los archivos  ubicados en sitios remotos, pero de cara al usuario es como si estuvieran en local.

Algunos de estos pueden ser:

1. SMB/CIFS
2. NFS
3. Coda
4. Lustre (que vimos en el ejercicio anterior)

#### SMB
Ventajas

- Buen soporte para uso compartido de archivos
- Acceso desde una amplia gama de clientes
- Mayor seguridad
- Sirve directorios e impresoras
- Autentifica conexiones a dominios Windows

Desventaja

- Falta encriptación en la capa de transporte

#### NFS
Ventajas

- Se reduce requerimientos de espacio en disco
- Se puede usar como complemento a NIS
- Puede utilizarse para proveer espacio de disco a estaciones que no tengan disco.
  
Desventaja

- Si un directorio se exporta como root, una persona con superprevilegios puede llegar a escribir en la raiz.
- Si se exporta sin lista de acceso, puede acceder cualquiera a el. 

#### CODA

Ventajas

 - Puede trabajar sin conexión
 - Es software libre
 - Gran rendimiento gracias a la caché persistente
 - Replica servidores
 - Modelo de seguridad para autenticació, cifrado y control de acceso.
 - Ajuta el ancho de banda en red
 - Escala bien


