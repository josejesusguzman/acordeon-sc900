# Explicación de cifrado

![Cifrado](/imgs/6-encryption.png)

El cifrado es una técnica esencial en la ciberseguridad que protege la información transformándola en un formato ilegible sin la clave adecuada. Su propósito es asegurar que los datos solo sean accesibles para las personas autorizadas, incluso si caen en manos equivocadas. Hay dos tipos principales de cifrado: simétrico y asimétrico. Cada uno tiene sus usos, ventajas y desventajas.


## Cifrado Simétrico
El cifrado simétrico utiliza la misma clave para cifrar y descifrar los datos. Piensa en ello como una caja fuerte con una cerradura que requiere la misma llave para abrirse y cerrarse. Este método es rápido y eficiente, ideal para cifrar grandes volúmenes de datos. Sin embargo, el principal desafío es la distribución segura de la clave, ya que cualquier persona con acceso a ella puede descifrar los datos.

Es como compartir una palabra secreta entre dos personas que quieren comunicarse en secreto. Ambos deben conocer la palabra secreta (clave) para entenderse, pero si alguien más la descubre, también puede entender el mensaje.

### Ejemplo de Implementación de Cifrado Simétrico

Un sistema de gestión de archivos empresarial que almacena archivos sensibles en un servidor o en la nube.

Cuando un empleado guarda un archivo en el sistema, el sistema automáticamente cifra el archivo usando una clave simétrica antes de almacenarlo. Esta clave es generada y gestionada por el propio sistema de gestión de archivos, y se asegura que sea única y fuertemente protegida.

1. El sistema genera una clave simétrica fuerte (por ejemplo, usando AES-256).
2. Antes de almacenar el archivo, el sistema cifra los datos del archivo usando esta clave.
3. El archivo cifrado se almacena en el servidor o la nube.
4. Cuando el empleado necesita acceder al archivo, el sistema descifra el archivo utilizando la misma clave.

**Ventaja**: La velocidad de cifrado y descifrado hace que este método sea ideal para el procesamiento de grandes volúmenes de datos.

### Ejemplo de Implementación de Cifrado Asimétrico

Un servicio de mensajería seguro utilizado para comunicaciones empresariales.

Cuando un empleado envía un mensaje a otro dentro de la organización, el sistema utiliza el cifrado asimétrico para asegurar que solo el destinatario pueda leer el mensaje.

1. Cada usuario tiene un par de claves asimétricas: una pública y una privada. La clave pública es accesible por cualquier persona dentro de la organización, pero la clave privada es mantenida en secreto por el usuario.
2. Cuando un empleado quiere enviar un mensaje seguro, cifra el mensaje utilizando la clave pública del destinatario.
3. El mensaje cifrado se envía a través de la red.
4. El destinatario utiliza su clave privada para descifrar el mensaje.

**Ventaja**: Este método asegura que solo el destinatario pueda descifrar y leer el mensaje, proporcionando una capa adicional de seguridad para la comunicación sensible.

| Característica       | Cifrado Simétrico                    | Cifrado Asimétrico                       |
|----------------------|--------------------------------------|-----------------------------------------|
| Tipo de Clave        | Una única clave para cifrar y descifrar| Par de claves: una pública y una privada |
| Velocidad            | Rápido                               | Más lento que el cifrado simétrico       |
| Uso                  | Adecuado para grandes volúmenes de datos| Intercambio seguro de claves, firmas digitales |
| Distribución de Clave| Difícil, requiere un canal seguro    | Fácil, la clave pública se puede compartir abiertamente |
| Ejemplo              | Cifrado de archivos en un disco duro | HTTPS en sitios web                      |
| Seguridad            | Fuerte, pero depende de la gestión segura de la clave | Muy fuerte, especialmente para el intercambio de claves |
