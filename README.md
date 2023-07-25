# JDox Jekyll Theme

[![Jekyll site CI](https://github.com/aliifam/jdox/actions/workflows/jekyll.yml/badge.svg?branch=master)](https://github.com/aliifam/jdox/actions/workflows/jekyll.yml)

# Nice commands

- bundle install
- jekyll serve
- gem install jekyll
- which ruby
- ruby -v
- echo $PATH

Si la ruta a la instalación de Ruby no está presente en la salida, puedes agregarla manualmente en el archivo .bashrc o .bash_profile en tu directorio de inicio de WSL. Agrega la siguiente línea al archivo:

export PATH="$PATH:/mnt/c/Ruby32-x64/bin" # Reemplaza "/mnt/c/Ruby32-x64/bin" con la ruta correcta a tu instalación de Ruby.

- ls /mnt/c/Ruby32-x64/bin/ruby

Ingresa el anterior comando para verificar el acceso al ejecutable de Ruby: Verifica que el archivo ejecutable de Ruby (ruby) se encuentre en la ruta especificada. Puedes verificarlo ejecutando:

- jekyll doctor
- jekyll doctor --verbose
- jekyll clean

# jekyll-livereload complement

Un comando que te permita tener un servidor local y ver los cambios reflejados en tiempo real mientras desarrollas tu sitio web, existe un complemento llamado jekyll-livereload.

jekyll-livereload es un complemento que agrega la funcionalidad de recarga en vivo (live-reload) a tu servidor local de Jekyll. Con este complemento, cada vez que realices cambios en tus archivos fuente, la página se actualizará automáticamente en el navegador sin necesidad de recargar manualmente.

Para utilizar jekyll-livereload, primero debes agregarlo a tu archivo Gemfile (si no lo tienes, créalo en la raíz de tu proyecto) y luego instalar las gemas mediante el siguiente comando:

- bundle install

Para crear un archivo Gemfile en la raíz de tu proyecto, puedes seguir estos pasos:

Abre tu terminal o línea de comandos.

Navega al directorio raíz de tu proyecto Jekyll utilizando el comando cd. Por ejemplo:

bash
Copy code
cd /ruta/de/tu/proyecto
Crea un archivo llamado Gemfile utilizando el editor de texto de tu preferencia. Por ejemplo, si utilizas el editor de texto Vim, puedes usar este comando:
bash
Copy code
vim Gemfile
Si prefieres utilizar otro editor de texto como Nano, puedes reemplazar "vim" con "nano" en el comando anterior.

Agrega las líneas necesarias en el archivo Gemfile para incluir el complemento jekyll-livereload y otras gemas que necesites. Por ejemplo:
ruby
Copy code
source "https://rubygems.org"
gem "jekyll"
gem "jekyll-livereload"

# Otras gemas que necesites

Guarda los cambios en el archivo Gemfile.

Luego, para instalar las gemas que has especificado en el archivo Gemfile, ejecuta el siguiente comando en la terminal:

- bundle install

Este comando instalará todas las gemas especificadas en el archivo Gemfile, incluyendo jekyll y jekyll-livereload.

Una vez que hayas realizado estos pasos, puedes ejecutar Jekyll con el comando jekyll serve --livereload para tener el servidor local con la funcionalidad de recarga en vivo habilitada.

Espero que esta explicación sea más clara y útil. Si tienes alguna otra pregunta o necesitas más ayuda, no dudes en preguntar. Estoy aquí para ayudarte.
