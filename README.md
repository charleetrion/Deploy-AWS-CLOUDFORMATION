# CLOUDFORMATION - Despliegue en AWS ECS con EC2

Este repositorio contiene archivos de configuración en YAML para desplegar servicios en AWS utilizando CloudFormation.

## 🚀 Descripción

El proyecto facilita la implementación de infraestructura en AWS, utilizando **ECS con instancias EC2**. Aquí encontrarás los archivos necesarios para crear y gestionar los recursos en AWS de manera automatizada.
Este despliegue incluye una aplicación desarrollada en **FastAPI**, empaquetada en una imagen de **Docker** y alojada en **AWS ECR**.

## 📂 Estructura del repositorio
* Cluster-Deploy.yml: Define el clúster ECS basado en instancias EC2, Autoscaling...
* VPC.yml :  Configura la VPC, subnets, rutas ...
* Service.yml: Creacion de **ListenerRuleHealthCheck**, **TaskDefinition**, **ECSService** ...
* ELB.yml: Define la configuración del **ALB**, **Grupo de Seguridad** y **Listener** ...

## 📌 Requisitos

Antes de desplegar estos archivos, asegúrate de tener:

- Una cuenta de **AWS** con permisos para utilizar CloudFormation, ECS y EC2.
- **AWS CLI** instalado y configurado con credenciales válidas.
- **Docker** instalado para construir la imagen de la aplicación.
- **FastAPI** instalado si deseas probar localmente la aplicación antes de desplegar.

### 📌 Notas

- Los parámetros como nombres de servicios, subnets y ARN de roles deben ajustarse según tu entorno.
- Revisa las dependencias entre archivos antes de desplegar.
- Puedes modificar las definiciones YAML según los requerimientos de tu proyecto.
- Asegúrate de actualizar la imagen en ECR antes de actualizar el stack.

📌 **Autor:** [charleetrion](https://github.com/charleetrion)  
🛠️ **Tecnologías:** AWS CloudFormation, ECS, EC2, Secrets Manager, Load Balancer, FastAPI, Docker
