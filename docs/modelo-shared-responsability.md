# Modelo de responsabilidad compartida

El modelo de responsabilidad compartida en Microsoft Azure es un concepto clave para entender cómo se dividen las responsabilidades de seguridad entre Microsoft y el cliente, dependiendo del tipo de servicio en la nube utilizado: On-premise, IaaS (Infraestructura como Servicio), PaaS (Plataforma como Servicio), y SaaS (Software como Servicio). Vamos a explorar cada uno con detalle, analogías y ejemplos para facilitar la comprensión.

![Modelo de responsabilidad compartida](/imgs/modelo-shared-respon.png)

## On-premise
Cuando operas On-premise, tienes el control total y, por lo tanto, la responsabilidad completa sobre todos los aspectos de tu infraestructura de TI. Es como tener una casa donde tú eres responsable del mantenimiento, desde la plomería hasta la seguridad.

![On-premise](/imgs/imagen-on-premise.webp)

## IaaS (Infraestructura como Servicio)
En IaaS, Microsoft proporciona la infraestructura básica (servidores, almacenamiento, redes), pero tú gestionas el sistema operativo, las aplicaciones y los datos. Es similar a alquilar un apartamento; el propietario se encarga del edificio y tú de lo que ocurre dentro de tu espacio.

![IaaS](/imgs/imagen-iaas.webp)

## PaaS (Plataforma como Servicio)
Con PaaS, Microsoft además de la infraestructura, se encarga del sistema operativo y de algunas configuraciones. Tu responsabilidad se centra en las aplicaciones y los datos. Esto es como un restaurante en un hotel donde te proporcionan la cocina y el comedor, pero tú aportas los chefs y el menú.

![PaaS](/imgs/imagen-paas.webp)

## SaaS (Software como Servicio)
En el modelo SaaS, Microsoft gestiona todo, desde la infraestructura hasta las aplicaciones. Solo eres responsable de gestionar tus datos y el acceso de los usuarios. Es similar a pedir comida a domicilio; simplemente disfrutas de la comida sin preocuparte por cocinar o limpiar.

![SaaS](/imgs/imagen-saas.webp)

Ahora, veamos una tabla resumen:

| Característica | On-premise       | IaaS                | PaaS                | SaaS                |
|----------------|------------------|---------------------|---------------------|---------------------|
| Infraestructura| Cliente          | Microsoft           | Microsoft           | Microsoft           |
| Sistema Operativo| Cliente       | Cliente             | Microsoft           | Microsoft           |
| Aplicaciones  | Cliente          | Cliente             | Cliente             | Microsoft           |
| Datos         | Cliente          | Cliente             | Cliente             | Cliente             |
| Actualizaciones| Cliente         | Cliente/Parcialmente Microsoft | Microsoft | Microsoft |
| Control       | Completo por el cliente | Control compartido | Menor control por el cliente | Microsoft |
| Ejemplo       | Servidor físico en tu empresa | VMs en Azure | Azure SQL Database | Office 365          |


- **On-premise**: Tienes el control total, pero también todas las responsabilidades.
- **IaaS**: Te permite ser flexible con la infraestructura sin la necesidad de hardware físico, manteniendo un alto grado de control sobre tus sistemas operativos y aplicaciones.
- **PaaS**: Facilita el desarrollo de aplicaciones sin preocuparte por el sistema operativo, la infraestructura o incluso algunas configuraciones de la aplicación.
- **SaaS**: Ofrece la solución más libre de preocupaciones, donde principalmente gestionas el acceso y los datos, ideal para aplicaciones que requieren poco a ningún control personalizado.