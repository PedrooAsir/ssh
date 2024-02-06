# SSH

## 1. **Conectarse al usuario admin de otra máquina por medio de claves publica y privado.**

- Empezamos generando una clave con el comando **ssh-keygen**. 

(Cabe recalcar que el SSH tiene que estar instalado). A continuación nos dirá en que ruta se guardará (/.ssh) en el que también la podemos poner a nuestro gusto. 

Si la queremos por defecto simplemente pulsamos "Enter" y nos pedirá si queremos poner una *passphrase* que es como una capa mas de seguridad, eso ya al gusto del consumidor. Obviamente si no la queremos pues no ponemos nada.

*Si vamos a la carpeta donde se almacenan las claves /home/asir2/.ssh/id_rsa o id_rsa.pub* , dependiendo si quieres la pública (**.pub**) o la privada.


A la otra persona le compartiremos la clave pública que se almacena en el archivo **id_rsa.pub**. Para ello haremos lo siguiente -->

- Continuamente, pondremos el comando **ssh-copy-id [usuario]@[IP a la que quieres conectarte]**


## 2. **Como configurar el acceso ssh en el GitHub.**
