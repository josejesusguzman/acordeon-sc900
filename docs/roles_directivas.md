# Roles VS directivas

Al profundizar en el mundo de la ciberseguridad dentro de Microsoft Azure, es crucial entender las diferencias y aplicaciones entre los roles de Microsoft Entra ID (anteriormente conocido como Azure Active Directory o Azure AD) y las directivas de Azure Policy. Ambos juegan roles vitales pero distintos en la gestión y la seguridad de los recursos en la nube.


## Roles de Microsoft Entra ID

Los roles de Microsoft Entra ID están diseñados para administrar permisos y accesos a recursos dentro de Azure Active Directory. Piensa en estos roles como los distintos sombreros que los miembros de un equipo podrían usar en un restaurante. Al igual que un chef tiene permisos para acceder a la cocina y preparar los alimentos, pero no necesariamente para servir mesas, los roles en Azure AD asignan permisos específicos a los usuarios basados en sus necesidades de acceso y responsabilidades laborales. Esto ayuda a asegurar que los usuarios tengan acceso solo a los recursos que necesitan para realizar su trabajo, reduciendo el riesgo de acceso no autorizado a datos sensibles.

## Directivas de Azure Policy

Por otro lado, las directivas de Azure Policy se utilizan para definir reglas y cumplir con los estándares de la organización en toda la infraestructura de Azure. Siguiendo con la analogía del restaurante, si consideramos las regulaciones de salud y seguridad como las directivas, estas directivas garantizarían que todos los procesos, desde la preparación de alimentos hasta la limpieza, cumplan con ciertos estándares. En el contexto de Azure, las directivas pueden forzar la implementación de ciertos estándares de seguridad, como asegurar que todos los discos duros virtuales estén cifrados, o que ciertos servicios solo estén accesibles desde ubicaciones geográficas específicas.


| Aspecto                 | Roles de Microsoft Entra ID              | Directivas de Azure Policy                   |
|-------------------------|------------------------------------------|---------------------------------------------|
| Finalidad               | Asignar permisos específicos a usuarios. | Garantizar el cumplimiento de estándares.   |
| Enfoque                 | Acceso y seguridad a nivel de usuario.   | Cumplimiento y configuración a nivel de recursos. |
| Ejemplo de uso          | Otorgar a un empleado acceso a Azure AD. | Forzar el cifrado de discos duros virtuales.|
| Aplicación              | A nivel de identidad y acceso.           | A nivel de infraestructura y recursos.      |
| Analogía                | Los diferentes puestos en un equipo de restaurante. | Regulaciones de salud y seguridad en un restaurante.|
| Control                | Basado en el rol del usuario.            | Basado en las políticas de la organización. |
| Similitud              | Ambos mejoran la seguridad y gestión.    | Ambos se utilizan para controlar y administrar cómo se accede y utiliza Azure. |
