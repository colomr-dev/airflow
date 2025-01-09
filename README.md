# Apache Airflow

Este repositorio está dedicado a **pruebas y laboratorios** realizados para aprender y profundizar en **Apache Airflow**, una herramienta clave para la orquestación de flujos de trabajo. Fue utilizado como parte de mi preparación para la certificación **Google Professional Data Engineer**, donde trabajé con **GCP Cloud Composer**, un servicio basado en Apache Airflow.

## Contexto

Durante mi preparación para la certificación, decidí instalar y configurar Apache Airflow en una distribución de **Ubuntu 22.04**. Esto me permitió:
- Comprender en profundidad cómo funciona Apache Airflow antes de usarlo como servicio gestionado en **Google Cloud Composer**.
- Realizar pruebas y laboratorios prácticos para explorar sus capacidades y limitaciones.

## Contenido del Repositorio

Este repositorio incluye:
- **DAGs de ejemplo**: Flujos de trabajo creados para probar diferentes funcionalidades de Airflow.
- **Configuraciones**: Archivos de configuración utilizados para instalar y ejecutar Apache Airflow en Ubuntu 22.04.
- **Pruebas**: Scripts y experimentos realizados para entender conceptos clave como:
  - Programación de tareas.
  - Integración con servicios externos.
  - Manejo de dependencias entre tareas.

## Instalación

Si deseas replicar el entorno utilizado, sigue estos pasos para instalar Apache Airflow en Ubuntu 22.04:

1. Actualiza los paquetes del sistema:
   ```bash
   sudo apt update && sudo apt upgrade
   ```
2. Instala los requisitos previos:
   ```bash
   sudo apt install python3-pip python3-venv
   ```
3. Crea un entorno virtual e instala Apache Airflow:
   ```bash
   python3 -m venv airflow_env
   source airflow_env/bin/activate
   pip install apache-airflow
   ```
4. Inicializa la base de datos y ejecuta el servidor web:
   ```bash
   airflow db init
   airflow webserver
   ```

## Uso

1. Accede a la interfaz web de Airflow en `http://localhost:8080`.
2. Carga los DAGs de ejemplo incluidos en este repositorio en el directorio `dags/`.
3. Ejecuta y monitorea los flujos de trabajo desde la interfaz.

## Recursos Adicionales

- [Documentación oficial de Apache Airflow](https://airflow.apache.org/docs/)
- [Google Cloud Composer](https://cloud.google.com/composer)
- [Guía de preparación para la certificación Google Professional Data Engineer](https://cloud.google.com/certification/data-engineer)

---

Este repositorio es parte de mi aprendizaje continuo en tecnologías de orquestación de datos y servicios en la nube. ¡Espero que también te sea útil si estás explorando Apache Airflow!