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

Do these steps once:

1. [Setup Github Locally](https://www.youtube.com/watch?v=hNUNPkoledI) (also see [_Happy Git and GitHub for the useR_](https://happygitwithr.com/github-acct.html))
2. Install {usethis} and {devtools} `install.packages(c("usethis", "devtools"))`
3. Set up a default {usethis} directory:
  - `usethis::edit_r_profile()` to open your profile for editing.
  - Add this line: `options(usethis.destdir = "YOURDIR")` (replace `YOURDIR` with the root directory under which you want your R projects to appear; or you can skip these steps, and the project will be saved to your Desktop).
  - Restart your R session (Session/Restart R in Rstudio).
4. `usethis::create_from_github("r4ds/bookclub-BOOKABBR")` (cleanly creates your own copy of this repository).

Do these steps each time you present another chapter:

1. Open your project for this book.
2. `usethis::pr_init("my-chapter")` (creates a branch for your work, to avoid confusion, making sure that you have the latest changes from other contributors; replace `my-chapter` with a descriptive name, ideally).
3. `devtools::install_dev_deps()` (installs any packages used by the book that you don't already have installed).
4. Edit the appropriate chapter file, if necessary. Use `##` to indicate new slides (new sections).
5. If you use any packages that are not already in the `DESCRIPTION`, add them. You can use `usethis::use_package("myCoolPackage")` to add them quickly!
6. Build the book! ctrl-shift-b (or command-shift-b) will render the full book, or ctrl-shift-k (command-shift-k) to render just your slide. Please do this to make sure it works before you push your changes up to the main repo!
7. Commit your changes (either through the command line or using Rstudio's Git tab).
8. `usethis::pr_push()` (pushes the changes up to github, and opens a "pull request" (PR) to let us know your work is ready).
9. (If we request changes, make them)
10. When your PR has been accepted ("merged"), `usethis::pr_finish()` to close out your branch and prepare your local repository for future work.
11. Now that your local copy is up-to-date with the main repo, you need to update your remote fork. Run `gert::git_push()` or click the `Push` button on the `Git` tab of Rstudio.

Cuando tu *PR* sea incorporado en el repositorio principal, el sitio con las notas será automáticamente renderizado para incluir tus cambios en [el sitio](https://r4ds.github.io/bookclub-tmwr_es/).
