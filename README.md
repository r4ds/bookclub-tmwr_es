# DSLC Modelado Tidy con R - Club de Lectura

¡Bienvenidxs al Club de Lectura de DSLC Modelado Tidy con R!

Estamos leyendo juntos el libro [Modelado Tidy con R](https://www.tmwr.org/) por Max Kuhn y Julia Silge.
Únete al canal [#book_club-tmwr](https://dslcio.slack.com/archives/C01H9SLA48M) en el [Slack de DSLC](https://dslc.io/join) para participar.
En paralelo a la lectura del libro, estamos produciendo [notas sobre el libro](https://r4ds.github.io/bookclub-tmwr_es/).

## Horario de reuniones

Si gustas presentar, por favor revisa la hoja electrónica correspondiente a tu cohorte (enlaces en la siguiente sección, y en el canal de Slack [#book_club-tmwr](https://dslcio.slack.com/archives/C01H9SLA48M))!

- Cohorte 1 (empezó el 2022-02-08, terminó el 2023-03-07): [Grabaciones de reuniones previas](https://www.youtube.com/playlist?list=PL3x6DOfs2NGhd1Gli-IANpVZ9z6Zz5AAu)


<hr>  

## Instrucciones sobre como presentar

Este repositorio está estructurado como un sitio [{bookdown}](https://CRAN.R-project.org/package=bookdown).
Para presentar, sigue estas instrucciones:

**Configuración inicial (solo debe hacerse una vez):**

1. [Configura Github localmente (en inglés)](https://www.youtube.com/watch?v=hNUNPkoledI) (también revisa el libro [Happy Git and GitHub for the useR](https://happygitwithr.com/github-acct.html))
2. Instala `{usethis}` y `{devtools}`, puedes hacer esto con el comando `install.packages(c("usethis", "devtools"))`
3. Configura un directorio por defecto para `{usethis}`:
  - Ejecuta `usethis::edit_r_profile()` para editar el archivo de configuración de tu perfil en RStudio.
  - Agrega la siguiente línea: `options(usethis.destdir = "TU_DIRECTORIO")` (reemplaza `TU_DIRECTORIO` con el directorio en el que quieres que tus proyectos de R sean guardados; alternativamente, puedes ignorar estos pasos y tus proyectos de R serán guardados en el Escritorio).
  - Reinicia tu sesión de R (`Session > Restart R` en Rstudio).
4. Ejecuta `usethis::create_from_github("r4ds/bookclub-tmwr_es")` (crea una nueva copia de este repositorio).

**Agregar un nuevo capítulo (sigue estos pasas cada vez):**

1. Abre tu proyecto de R para este libro (archivo `.Rproj`).
2. Ejecuta `usethis::pr_init("mi-capítulo")` (crea una nueva "rama" para tu trabajo, para evitar conflictos, esto garantiza que tú tienes la última versión de los cambios hechos por otros autores/contribuyentes; reemplaza `mi-capítulo` por un nombre descriptivo, idealmente).
3. Ejecuta `devtools::install_dev_deps()` (instala los paquetes usados por este libro que tú no tengas instalados localmente).
4. Edita el archivo correspondiente al nuevo capítulo, de ser necesario. Use `##` para crear una nueva "filmina/transparencia/diapositiva" (*slide* en inglés), para separ los contenidos en secciones.
5. Si utilizas algún paquete que no este listado en el archivo `DESCRIPTION`, agregalos. Por ejemplo, si usas un paquete llamado `mi-paquete-super-genial`, ejecuta el siguiente comando para agregarlo al archo `DESCRIPTION`, `usethis::use_package("mi-paquete-super-genial")`.
6. Construye/renderiza el libro. Para esto puedes usar la combinación de teclas: `ctrl-shift-b` (o `command-shift-b`), estos renderizaran una nueva versión del libro en su totalida. Alternativamente, puedes usar `ctrl-shift-k` (o `command-shift-k`) para renderizar solo tus "filminas/transparencias/diapositivas". Por favor, asegurate de seguir estos pasos antes de enviar los cambios al repositorio principal, esto garantizará que tus cambios tienen el formato correcto.
7. Envía tus cambios (puede ser unsando la línea de comandos o el menú de Git en RStudio).
8. Ejecuta `usethis::pr_push()` (empuja los cambios a el repositorio de GitHub y abre un *pull request* (PR), para hacernos saber que tu trabajo está listo).
9. (Si te solicitamos cambios, por favor hazlos)
10. Cuando tu PR sea aceptado ("combinado"), ejecuta `usethis::pr_finish()` para "cerrar" la "rama" en la que trabajaste los cambios y preparar tu repositorio local para cambios futuros.
11. Ahora que tu copia local está actualizada con el repositorio principal, tienes que actulizar to copia (*fork*) remota. Ejecuta `gert::git_push("origin")` o da click en el botón `Push` del menú Git en RStudio.

Cuando tu *PR* sea incorporado en el repositorio principal, el sitio con las notas será automáticamente renderizado para incluir tus cambios en [el sitio](https://r4ds.github.io/bookclub-tmwr_es/).
