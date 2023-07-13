Este repositorio es una prueba de helm con argocd. Tiene un esquema sencillo y funciones como toyaml, if else,range key value, default, quote, nindent, define (include)

Funcional y probado con minikube.

Tiene dos deployments que trabajan en dos servicios (escuchando en el puerto 80) con un pod cada uno, con containers con una imagen de nginx y otro de httpd escuchando en el 80. Además contiene un ingress configurado (para que puedas ir de un servicio a otro según el dominio, en el /etc/hosts debes poner 127.0.0.1 nombredominio, además de tener habilitado dos addons en minikube)

Requisitos, tener minikube instalado y helm.
Info config ingress
https://minikube.sigs.k8s.io/docs/handbook/addons/ingress-dns/