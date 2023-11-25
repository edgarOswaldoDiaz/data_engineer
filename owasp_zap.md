#### OWASP ZAP

Ejecutar en el entorno de consola (linux / Ms. PowerShell)

    podman run -u zap -p 8080:8080 -p 8090:8090 -i softwaresecurityproject/zap-stable zap-webswing.sh

Ejecutar en un web browser la url  

    http://localhost:8080/zap

Otros comando que pueden ayudar

    podman image ls # verifica las imágenes de los contenedores en el Registry local
    podman ps –a # verifica los contenedore habilitados en el host local

_______________________________________

> Referencia: https://www.zaproxy.org/download/
