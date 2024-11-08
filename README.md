# Proyecto TFG ASIR: Monitorización de la Red con Wazuh

**Titulación:** CFGS en Administración de Sistemas Informáticos en Red  
**Curso:** 2023/2024  

Este proyecto tiene como objetivo la implementación de un sistema de monitorización de red utilizando Wazuh para mejorar la seguridad de la infraestructura informática en una organización. La solución permite una detección temprana de amenazas, análisis de eventos de seguridad y respuestas automatizadas a incidentes en endpoints distribuidos en la red.

## Introducción
Este proyecto implementa Wazuh, una plataforma de código abierto de monitorización de seguridad que permite detectar y responder ante incidentes, proporcionando un entorno de seguridad más robusto para los sistemas de una empresa. 

Wazuh se despliega en un servidor principal que se conecta y monitorea los endpoints (clientes) de la red, analizando eventos de seguridad y aplicando respuestas automáticas ante actividades maliciosas.

## Finalidad del Proyecto
El proyecto se centra en:
1. Fortalecer la seguridad mediante una detección y respuesta temprana a amenazas.
2. Proveer visibilidad detallada de la actividad en los sistemas de la red.
3. Automatizar la gestión de seguridad y reducir el tiempo de respuesta ante incidentes.

## Objetivos del Sistema
- **Recopilación Continua de Eventos:** Monitoreo constante de la actividad en los endpoints.
- **Biblioteca de Eventos Forenses:** Almacenamiento centralizado de eventos de seguridad para su análisis.
- **Búsquedas Personalizadas de Amenazas:** Realización de análisis detallados y personalizados de seguridad.
- **Notificaciones Automatizadas:** Integración con Slack para recibir notificaciones de alertas críticas.

## Requisitos
### Hardware
- **Servidor Linux:** Donde se instala el servidor Wazuh (recomendado: Ubuntu Server 22.04 LTS).
  - **RAM:** 4 GB
  - **Almacenamiento:** 500 GB
- **Clientes:** Compatible con sistemas operativos Windows y Ubuntu.

### Software
- **Ubuntu Server 22.04 LTS**
- **Docker:** Para contenerizar y gestionar el servidor Wazuh.
- **Python:** Para automatizar tareas como el borrado de archivos maliciosos.
- **Slack y VirusTotal:** Para notificaciones y escaneo de amenazas.
- **Ansible:** Para gestionar la configuración de nuevos clientes en Linux.

## Arquitectura del Sistema
El sistema se despliega en un servidor central en Docker, y los clientes son configurados para enviar eventos a este servidor. Las alertas se gestionan y notifican en tiempo real a través de integraciones con herramientas externas como Slack.
