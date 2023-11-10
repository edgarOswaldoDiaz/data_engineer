### Data engineer (Plataforma para ingeniería de datos masivos)

#### Contenedor basado en IDE Juppyter Lab (Python & R Kernel).
    podman pull jupyter/datascience-notebook

#### Contenedor basado en Visualización Apache Superset.
    podman pull apache/superset

#### Contenedor basado en Apache NiFi
    podman pull apache/nifi

#### Contenedor basado en Apache Jmeter
    podman pull justb4/jmeter
    podman run --name ${NAME} -i -v ${LOCAL_PLUGINS_FOLDER}:/plugins -v ${LOCAL_JMX_WORK_DIR}:${CONTAINER_JMX_WORK_DIR} -w ${PWD} ${IMAGE} $@
----------
- Download Podman Desktop https://podman-desktop.io/ 
