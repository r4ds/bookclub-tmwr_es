# R4DS Modelado Tidy con R - Club de Lectura

¡Bienvenidxs al Club de Lectura de R4DS Modelado Tidy con R!

Estamos leyendo juntos el libro [Modelado Tidy con R](https://www.tmwr.org/) por Max Kuhn y Julia Silge.
Únete al canal [#book_club-tmwr](https://rfordatascience.slack.com/archives/C01H9SLA48M) en el [Slack de R4DS](https://r4ds.io/join) para participar.
En paralelo a la lectura del libro, estamos produciendo [notas sobre el libro](https://r4ds.github.io/bookclub-tmwr_es/).

## Horario de reuniones

Si gustas presentar, por favor revisa la hoja electrónica correspondiente a tu cohorte (enlaces en la siguiente sección, y en el canal de Slack [#book_club-tmwr](https://rfordatascience.slack.com/archives/C01H9SLA48M))!

- [Cohorte 1](https://docs.google.com/spreadsheets/d/1apDY5yyimVUwebhZvTwM3P7Pysa9ztZvj4EUF_KFVdw/edit#gid=0) (empezó el 2022-02-08): [Martes, 4:00pm CST/CDT (GMT-6/5)](https://www.timeanddate.com/worldclock/converter.html?iso=20220531T210000&p1=24) | [Grabaciones de reuniones previas](https://www.youtube.com/playlist?list=PL3x6DOfs2NGhd1Gli-IANpVZ9z6Zz5AAu)


<hr>  

## Instrucciones sobre como presentar

Este repositorio está estructurado como un sitio [{bookdown}](https://CRAN.R-project.org/package=bookdown).
Para presentar, sigue estas instrucciones:

1. [Configura GitHub localmente](https://www.youtube.com/watch?v=hNUNPkoledI) (en inglés).
2. Haz un *fork* (crea una copia en tu cuenta personal) de este repositorio.
3. Crea un nuevo proyecto en RStudio (`File > New Project > Version Control`) con este *fork*.
4. Instala las dependencias de este libro con el comando `devtools::install_dev_deps()` (técnicamente este paso es opcional, pero necesitas las dependencias para renderizar el libro completo, de forma local).
5. Crea una nueva rama (*branch*) en tu *fork* para incluir tus cambios.
6. Edita el archivo del capítulo apropiado. Usa `##` para crear nuevas secciones dentro del capítulo.
7. Si usas paquetes adicionales, no incluídos en el archivo llamado `DESCRIPTION`, agrégalos. Puedes usar el comando `usethis::use_package("miPaquete")` para agregarlos rápidamente.
8. Registra tus cambios haciendo un *commit*.
9. Empuja tus cambios a tu rama (*branch*) en tu *fork* de GitHub.
10. Abre un *pull request (PR)* para hacernos saber que hay cambios listos, para ser incorporados en el repositorio principal.

Cuando tu *PR* sea incorporado en el repositorio principal, el sitio con las notas será automáticamente renderizado para incluir tus cambios en [el sitio](https://r4ds.github.io/bookclub-tmwr_es/).
