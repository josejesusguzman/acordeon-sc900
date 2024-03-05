# Zero Trust

El modelo de Confianza Cero (Zero Trust) es un enfoque de seguridad que Microsoft Azure y muchas otras plataformas y organizaciones están adoptando para proteger sus datos y sistemas. Este modelo se fundamenta en la premisa de "nunca confiar, siempre verificar", lo cual es esencial en el contexto de la certificación SC-900: Microsoft Security, Compliance, and Identity Fundamentals. Este modelo contrasta con los enfoques tradicionales de seguridad en los que se asume que todo lo que está dentro de la red corporativa es seguro.

![Zero Trust](/imgs/2-zero-trust-pillars-v2.png)

## Pilares del Zero Trust
El modelo de Confianza Cero se basa en tres pilares fundamentales:

1. **Verificar explícitamente**: Cada solicitud de acceso, independientemente de dónde provenga o a qué recurso intente acceder, debe ser verificada rigurosamente. Esto implica la autenticación y autorización de usuarios basada en toda la información disponible, incluyendo su identidad, la ubicación, el tipo de dispositivo, la salud del dispositivo, y más.

2. **Usar el menor privilegio necesario**: Este principio se centra en limitar el acceso solo a los recursos necesarios para realizar una tarea específica. Esto minimiza el riesgo de que un atacante pueda acceder a información sensible o crítica a través de una cuenta comprometida.

3. **Suponer una violación**: Bajo el modelo de Confianza Cero, se asume que los atacantes pueden estar dentro de la red en cualquier momento. Esto implica la necesidad de segmentar los recursos y controlar el movimiento lateral dentro de la red, además de implementar estrategias robustas de detección y respuesta a incidentes.

## Implementación
La implementación del modelo de Confianza Cero involucra varios componentes y prácticas clave:

- **Identidad como el nuevo perímetro de seguridad**: Dado que las aplicaciones y los datos pueden estar en cualquier lugar (no solo dentro de la red corporativa), la identidad del usuario se convierte en el eje central de la política de seguridad. Esto implica la implementación de soluciones de gestión de identidades y accesos, como Azure Active Directory, con capacidades como la autenticación multifactor (MFA) y la gestión de identidades privilegiadas.

- **Protección de los datos**: Encriptación tanto en tránsito como en reposo, clasificación de datos, y políticas de prevención de pérdida de datos (DLP) son esenciales para proteger la información sensible en cualquier ubicación.

- **Seguridad de las aplicaciones y la red**: Asegurar las conexiones entre aplicaciones, datos, y usuarios requiere de soluciones como firewalls, protección contra amenazas avanzadas (como Microsoft Defender for Endpoint), y el uso de redes privadas virtuales (VPNs) o acceso seguro a la red basado en el contexto del acceso (SDP).

- **Automatización y orquestación**: La automatización de respuestas a incidentes y la orquestación de políticas de seguridad a través de herramientas y plataformas permiten una respuesta más rápida y eficiente a las amenazas.

## Ejemplos de Aplicación
- **Control de Acceso Basado en Roles (RBAC)**: Limitar el acceso a recursos basado en el rol del usuario dentro de la organización, asegurando que solo puedan acceder a lo que necesitan para sus funciones específicas.

![RBAC](/imgs/rbac-overview.png)

- **Microsegmentación**: Dividir la red en zonas seguras para controlar el acceso y el movimiento dentro de la red, lo que ayuda a contener las amenazas y minimizar el daño potencial.

- **Políticas de seguridad dinámicas**: Utilizar la inteligencia artificial y el análisis de comportamiento para adaptar las políticas de seguridad en tiempo real basadas en el contexto del acceso y la evaluación continua de riesgos.