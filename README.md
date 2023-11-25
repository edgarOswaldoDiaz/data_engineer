### Data engineer (Plataforma para ingeniería de datos masivos)

#### Contenedor basado en IDE Juppyter Lab (Python & R Kernel).
    podman pull jupyter/datascience-notebook

#### Contenedor basado en Visualización Apache Superset.
    podman pull apache/superset

#### Contenedor basado en Apache NiFi
    podman pull apache/nifi

#### Contenedor basado en Apache Jmeter
    podman pull justb4/jmeter

#### Activar
    podman run --name ${NAME} -i -v ${LOCAL_PLUGINS_FOLDER}:/plugins -v ${LOCAL_JMX_WORK_DIR}:${CONTAINER_JMX_WORK_DIR} -w ${PWD} ${IMAGE} $@

#### Contenedor basado en Owasp ZAP

    sudo podman pull owasp/zap2docker-stable

Crear un archivo owasp_zap.sh y dar atributos para permitir ejecución, con el siguiente contenido.

    podman run -u zap -p 8086:8080 -p 8091:8090 -i owasp/zap2docker-stable zap-webswing.sh

Nota: Acceder a la herramienta por medio de un web browser con http://IP-asignada:8086/zap

----------
- Download Podman Desktop https://podman-desktop.io/ 
