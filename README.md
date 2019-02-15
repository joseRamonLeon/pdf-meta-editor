# pdf-meta-editor Edita los metadatos de un PDF

[![version (npm)](https://img.shields.io/npm/v/pdf-meta-editor.svg?style=flat-square)](https://www.npmjs.com/package/pdf-meta-editor)
[![license (GitHub)](https://img.shields.io/github/license/Scriptim/pdf-meta-editor.svg?longCache=true&style=flat-square)](https://github.com/Scriptim/pdf-meta-editor/blob/master/LICENSE.md)
[![downloads (npm)](https://img.shields.io/npm/dt/pdf-meta-editor.svg?style=flat-square)](https://www.npmjs.com/package/pdf-meta-editor)
[![dependencies (libraries.io)](https://img.shields.io/librariesio/release/npm/pdf-meta-editor.svg?style=flat-square)](https://libraries.io/npm/pdf-meta-editor)

Cliente Interactivo para editar los metadatos de ficheros PDF

![Demo](demo.gif "Demo")

<https://www.npmjs.com/package/pdf-meta-editor>

## Instalación

    sudo npm install -g pdf-meta-editor

## Uso

    pdf-meta-editor FILENAME

### Argumentos desde Línea de Comandos

#### `-h/--help`

Show this help page.

    $ pdf-meta-editor --help
    pdf-meta-editor

    Usage: pdf-meta-editor FILENAME [-p|-o]
           pdf-meta-editor (-h|-v)

    options
      -h --help      Show this help page.
      -v --version   Print the currently installed version.
      -p --print     Print the metadata instead of editing it.
      -o --overwrite Overwrite the original file.

#### `-v/--version`

Imprime la versión actual instalada.

#### `-p/--print`

Muestra la información de los metadatos sin capacidad de edición.

##### Ejemplo

    $ pdf-meta-editor Demo.pdf --print
    Printing metadata of file Demo.pdf

    FileType: PDF
    FileSize: 5.7 kB
    FileModifyDate: 2018:07:13 00:00:00+00:00
    FileAccessDate: 2018:07:13 12:00:00+00:00
    FilePermissions: rw-r--r--
    PDFVersion: 1.3
    PageCount: 1
    Linearized: No

    Title: Demo Title
    Author: Demo Author
    Subject: Demo Subject
    CreateDate: 2018:07:13 00:00:00
    FileModifyDate: 2018:07:13 00:00:00+00:00
    Creator: Demo Creator
    Producer: Demo Producer
    Keywords: demo,pdf,file

#### `-o/--overwrite`

Sobreescribe el fichero original

Si no se especifica, el archivo original se conserva de forma predeterminada.
