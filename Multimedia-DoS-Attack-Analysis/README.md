# Análisis de Incidente: Ataque DoS por Inundación ICMP 🛡️

Este proyecto es una aplicación práctica realizada como parte del **Certificado Profesional de Ciberseguridad de Google**. El objetivo es demostrar la capacidad de un analista para gestionar un incidente de seguridad real utilizando el marco de trabajo **NIST Cybersecurity Framework (CSF)**[cite: 3, 4].

## 📝 Escenario del Incidente
Una empresa multimedia que ofrece servicios de diseño y marketing sufrió un ataque de Denegación de Servicio (**DoS**) que inhabilitó su red interna durante dos horas. 

*   **Problema**: Los servicios dejaron de responder debido a una avalancha masiva de paquetes ICMP entrantes (pings).
*   **Causa Raíz**: Un cortafuegos (firewall) mal configurado que permitía el paso de tráfico sin restricciones, lo que permitió al atacante saturar el ancho de banda de la organización.

## ⚙️ Metodología: Aplicación del NIST CSF
Para resolver este incidente y fortalecer la red, se aplicaron las cinco funciones del núcleo del NIST:

### 1. Identificar (Identify)
*   **Auditoría**: Se identificó que la brecha de seguridad se originó en una regla de firewall inexistente para el protocolo ICMP.
*   **Impacto**: El tráfico legítimo interno no pudo acceder a ningún recurso de red, afectando la productividad de todos los departamentos.

### 2. Proteger (Protect)
Se implementaron salvaguardas técnicas inmediatas para mitigar futuras amenazas:
*   **Limitación de Tasa (Rate Limiting)**: Nueva regla en el firewall para restringir el volumen de paquetes ICMP entrantes.
*   **Filtro Anti-Spoofing**: Verificación de direcciones IP de origen para bloquear paquetes con identidades falsificadas.

### 3. Detectar (Detect)
Se mejoraron las capacidades de monitoreo para aumentar la rapidez de detección:
*   **Monitoreo de Red**: Instalación de software especializado para alertar sobre patrones de tráfico anómalos.
*   **IDS/IPS**: Implementación de un sistema de detección y prevención de intrusiones para filtrar tráfico ICMP basado en firmas sospechosas.

### 4. Responder (Respond)
Acciones ejecutadas por el equipo de gestión de incidentes durante la crisis:
*   Bloqueo inmediato de paquetes ICMP entrantes para detener la saturación.
*   Desconexión de servicios de red no críticos para liberar recursos y restaurar primero los servicios vitales.

### 5. Recuperar (Recover)
*   Restauración del funcionamiento normal de todos los servicios de diseño y marketing una vez validada la seguridad de la red.
*   Verificación de que el tráfico interno puede acceder nuevamente a los recursos sin interrupciones.

---

## 🛠️ Herramientas y Habilidades Aplicadas
*   **Análisis de Protocolos**: Comprensión de ICMP y ataques de inundación (Flooding).
*   **Configuración de Seguridad**: Reglas de Firewall, IDS, IPS y Anti-spoofing.
*   **Cumplimiento y Marcos de Trabajo**: Aplicación proactiva y reactiva del NIST CSF.
*   **Documentación Técnica**: Redacción de informes de análisis de incidentes profesionales.

---
*Nota: Este análisis se basa en un escenario de entrenamiento proporcionado por Google para la formación en ciberseguridad.*
