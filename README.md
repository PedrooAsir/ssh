# SSH

## 1. **Conectarse al usuario admin de otra máquina por medio de claves publica y privado.**

- Empezamos generando una clave con el comando **ssh-keygen**. 

(Cabe recalcar que el SSH tiene que estar instalado). A continuación nos dirá en que ruta se guardará (/.ssh) en el que también la podemos poner a nuestro gusto. 

Si la queremos por defecto simplemente pulsamos "Enter" y nos pedirá si queremos poner una *passphrase* que es como una capa mas de seguridad, eso ya al gusto del consumidor. Obviamente si no la queremos pues no ponemos nada.

*Si vamos a la carpeta donde se almacenan las claves /home/asir2/.ssh/id_rsa o id_rsa.pub* (dependiendo si quieres la pública (**.pub**) o la privada). Tendremos los archivos de estas donde se almacenan las claves en la ruta especificada.


A la otra persona le compartiremos la clave pública que se almacena en el archivo **id_rsa.pub**. Para ello haremos lo siguiente -->

- Continuamente, pondremos el comando **ssh-copy-id [usuario al que te quieres conectar]@[IP a la que quieres conectarte]**

Con esto ya podremos conectarnos a la máquina de la otra persona , con el siguiente comando.

```
ssh [usuario al que te quieres conectar]@[IP de esa persona]

```

## 2. **Como configurar el acceso ssh en el GitHub.**

- En GitHUb vamos a *Settings* y vamos al apartado de SSH, donde añadiremos una clave SSH (add SSH key).

Ahí pondremos nuestra clave pública SSH, que se ubica en **/.ssh** y veremos el contenido del archivo *id_rsa.pub*.

Tan solo copiamos la clave generada que se encuentra dentro del archivo especificado y la pegamos en GitHub en el sitio especificado anteriormente.