#### OWASP ZAP

Ejecutar en el entorno de consola (linux / Ms. PowerShell)

    podman –version     # verifica la versión instalada de Docker  
    podman pull owasp/zap2docker-stable # descarga el contenedor de OWASP ZAP
    podman image ls # verifica las imágenes de los contenedores en el Registry local
    podman ps –a # verifica los contenedore habilitados en el host local
    podman run -u zap -p 85:8080 -p 8090:8090 -i owasp/zap2docker-stable zap-webswing.sh # habilita el contenedor local

Ejecutar en un web browser la url  

    http://localhost:85/zap
_______________________________________

> Referencia: owasp.org
