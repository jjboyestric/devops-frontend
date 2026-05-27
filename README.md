# DevOps Frontend - Innovatech Chile

## Descripción

Este repositorio contiene el Frontend del proyecto desarrollado para Innovatech Chile, correspondiente a la Evaluación Parcial N°2 de Introducción a Herramientas DevOps.

El Frontend fue desarrollado con React y Vite, y se encuentra contenedorizado mediante Docker. La aplicación se despliega en una instancia EC2 pública de AWS, siendo el único componente accesible desde Internet.

## Tecnologías utilizadas

- React
- Vite
- Docker
- Nginx
- GitHub Actions
- Docker Hub
- AWS EC2

## Arquitectura del servicio

El Frontend se ejecuta en una instancia EC2 pública. Desde esta instancia se permite la comunicación hacia los servicios Backend ubicados en una instancia privada dentro de la misma VPC.

La arquitectura general es:

```text
Internet
   |
   v
EC2 Frontend pública
   |
   v
EC2 Backend privada
