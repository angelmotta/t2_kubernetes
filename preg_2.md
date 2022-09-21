## Funcionalidad
La funcionalidad de la aplicación es recibir un HTTP request y retornar el nombre del host (hostmane) y la dirección
IP (IP) de la máquina o contenedor que está recibiendo y procesando el HTTP request.

## Finalidad
Esta funcionalidad es de gran ayuda cuando se utilizan múltiples nodos en una aplicación, ya que se puede visualizar
el balanceo de carga entre los 'n' nodos que tenga el clúster de la aplicación. Esto debido a que cada vez que se
envíe un request a la aplicación, esta responderá desde cualquiera de los nodos, permitiendo diferenciar en qué nodo
se está procesando el request, ya que la respuesta cambiará dependiendo del nodo que responda.

## Referencias
### GitHub
La implementación de la aplicación se encuentra en el siguiente repositorio de GitHub:

[pbitty/hello-from: A simple HTTP service that responds with its hostname and IP addresses](https://github.com/pbitty/hello-from)

### DockerHub
La imagen de la aplicación se encuentra en el siguiente repositorio de DockerHub:

[pbitty/hello-from:latest | Docker Hub](https://hub.docker.com/layers/pbitty/hello-from/latest/images/sha256-815b60bcc226e5e8c43f5d97f778238cd96937e1e0b34da00881b3881cbfbd08?context=explore)