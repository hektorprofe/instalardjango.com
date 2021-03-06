---
description: Videotutoriales de instalación y creación de entornos virtuales vía Conda para instalar Django Framework fácilmente en Windows, GNU/Linux y Mac OS X.
---
<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; height: auto; margin-bottom: 1rem; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style>
## Instalar Django fácilmente en entorno virtual Conda

Instalar Django en un entorno virtual nunca había sido tan fácil gracias a ***Conda***, un gestor de paquetes y entornos para multitud de lenguajes (Python, R, Ruby, Lua, Scala, Java, JavaScript, C/ C++, FORTRAN). En este videotutorial te enseñaré a instalar conda con ***Miniconda***, a crear tu primer entorno virtual y a instalar Django de una forma cómoda y sencilla. 

Si tienes algún problema durante la instalación [ábreme un ticket](https://github.com/hcosta/instalardjango.com/issues){:target="_blank"} y lo verificamos. {% comment %} pero si prefieres utilizar ***Virtualenv*** [aquí](virtualenv.md) encontrarás un manual.{% endcomment %}

***NOTA***: *Si dispones de Anaconda no es necesario instalar Miniconda, pues es una versión ligera del mismo programa. Puedes saltarte la instalación e ir directamente al paso de crear el entorno virtual.*

## Selecciona tu sistema operativo

<div style="text-align:center;">
  <a href="#win10"><img src="{{ '/assets/img/Logo_Windows_10.png' | relative_url }}" /></a>
  <a href="#mac"><img src="{{ '/assets/img/Logo_MacOS.png' | relative_url }}" /></a>
  <a href="#linux"><img src="{{ '/assets/img/Logo_Linux.png' | relative_url }}" /></a>
</div><a name="win7"></a>

<a name="win10"></a>
### Windows 10 
<div class='embed-container'><iframe src='https://player.vimeo.com/video/254713961' frameborder='0' webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe></div>

#### Chuleta de comandos en Windows 10
```bash
# Consultar la versión de Python por defecto
python -V

# Crear entorno Conda vacío con Python 3.7
conda create -n django2 python==3.7 sqlite==3.25.3

# Activar el entorno virtual
activate django2

# Listar los paquetes instalados en el entorno virtual
(django2) pip list

# Instalar Django en el entorno virtual
(django2) pip install django  # se puede instalar cualquier versión con django==2.0.2 o la que sea

# Crear un proyecto de Django
(django2) django-admin startproject proyecto

# Desinstalar Django del entorno virtual
(django2) pip uninstall django

# Desactivar el entorno virtual
(django2) deactivate
```
<a name="mac"></a>
### MacOS X 
<div class='embed-container'><iframe src='https://player.vimeo.com/video/254727538' frameborder='0' webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe></div>

#### Chuleta de comandos en MacOS X 
```bash
# Consultar la versión de Python por defecto
python -V

# Instalar un script bash del directorio actual
sh ./script.sh

# Inyectar la nueva configuración en el .bash_profile
source ~/.bash_profile

# Crear entorno Conda vacío con Python 3.7
conda create -n django2 python==3.7 sqlite==3.25.3

# Activar el entorno virtual
source activate django2

# Listar los paquetes instalados en el entorno virtual
(django2) pip list

# Instalar Django en el entorno virtual
(django2) pip install django  # se puede instalar cualquier versión con django==2.0.2 o la que sea

# Crear un proyecto de Django
(django2) django-admin startproject proyecto

# Desinstalar Django del entorno virtual
(django2) pip uninstall django

# Desactivar el entorno virtual
(django2) source deactivate
```
<a name="linux"></a>
### GNU/Linux 
<div class='embed-container'><iframe src='https://player.vimeo.com/video/254740303' frameborder='0' webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe></div>

#### Chuleta de comandos en GNU/Linux
```bash
# Consultar la versión de Python por defecto
python -V

# Instalar un script bash del directorio actual
sh ./script.sh

# Inyectar la nueva configuración en el .bashrc
source ~/.bashrc

# Crear entorno Conda vacío con Python 3.7
conda create -n django2 python==3.7 sqlite==3.25.3

# Activar el entorno virtual
source activate django2

# Listar los paquetes instalados en el entorno virtual
(django2) pip list

# Instalar Django en el entorno virtual
(django2) pip install django  # se puede instalar cualquier versión con django==2.0.2 o la que sea

# Crear un proyecto de Django
(django2) django-admin startproject proyecto

# Desinstalar Django del entorno virtual
(django2) pip uninstall django

# Desactivar el entorno virtual
(django2) source deactivate
```

## ¿Necesitas un IDE para Python y Django?

[Aquí encontrarás](visualstudiocode.md) un videotutorial de configuración paso a paso para **Visual Studio Code**, mi entorno de trabajo recomendado.
