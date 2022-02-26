# R4DS Modelado Tidy con R - Club de Lectura

¡Bienvenidxs al Club de Lectura de R4DS Modelado Tidy con R!

Estamos leyendo juntos el libro [Modelado Tidy con R](https://www.tmwr.org/) por Max Kuhn y Julia Silge.
Únete al canal `#book_club-tidy_modeling_with_r` en el [Slack de R4DS](https://r4ds.io/join) para participar.
En paralelo a la lectura del libro, estamos produciendo [notas sobre el libro](https://r4ds.github.io/bookclub-tmwr_es/).

## Horario de reuniones

Si gustas presentar, por favor agrega tu nombre al lado del capítulo usando el [Editor Web de GitHub](https://youtu.be/d41oc2OMAuI) (guía en inglés).

*Cohorte 1: Martes, 4:00pm CST/CDT (GMT-6)*

<details>
  <summary> Reuniones pasadas </summary>
- 2022-02-01: Bienvenida - Esmeralda Cruz-Silva y [Roberto Villegas-Diaz](https://github.com/villegar)
- 2022-02-08: Capítulo 1 - Software para modelado: [Roberto Villegas-Diaz](https://github.com/villegar)
- 2022-02-15: Capítulo 2 - Una cartilla tidyverse: Armando Ocampo
- 2022-02-22: Capítulo 3 - Una revisión de fundamentos de modelado en R: Esmeralda Cruz-Silva
</details>

**Reuniones futuras:**

- 2022-03-01: Extra - Revisión de Tidyverse (`purrr`, `dplyr`, etc.): [Roberto Villegas-Diaz](https://github.com/villegar)
- 2022-03-08: Capítulo 4 - Datos sobre casas Ames: Diana García
- 2022-03-15: Capítulo 5 - Gastando/usando nuestros datos: Armando Guzman
- 2022-03-22: Capítulo 6 - Ingeniería de características usando el paquete `recipes`: PENDIENTE
- 2022-04-05: Capítulo 7 - Ajustando models con el paquete `parsnip`: PENDIENTE
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

