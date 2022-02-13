# ProfLycee
Package, sans prétention, pour quelques commandes LaTeX utiles au lycée !

Pour le moment :

- deux macros pour créer, dans un environnement TikZ, des courbes d'interpolations et des tangentes ;
- deux macros pour configurer un environnement de Calcul Formel et pour créer les lignes ;
- un environnement pour présenter du code python (via pythontex) ;
- un environnement pour exécuter du code python et présenter le résultat dans une <i>console</i>.

## Courbe d'interpolation

La commande <code>\splinetikz[...]</code>, trace un ensemble de <i>splines</i> grâce notamment à une liste de points sous la forme <code>x1/y1/d1§x2/y2/d2§...</code> et une liste des coefficients de <i>compensation</i> sous la forme <code>C1G/C1D§C2G/C2D§...</code> (qui peut être simplifiée si on le souhaite !).

Également de quoi tracer, grâce à la commande <code>\tangentetikz[...]</code>, (une ou) des tangentes à l'aide de triplets <code>xa/ya/da§...</code> pour tracer une (portion de) tangente via <code>da*(x-xa)+ya</code>.

![illustr](proflycee-test-splines.png?raw=true "testsplines")

## Émulation fenêtre de calcul formel

Une commande <code>\paramCF[...]</code> pour paramétrer la *fenêtre de travail* du calcul formel.

Une commande <code>\ligneCF[...]</code> pour créer les lignes de la *fenêtre de travail*.

![illustr](proflycee-test-calcformel.png?raw=true "testcalc")

## Code et console Python

Un environnement <code>envcodepythontex[...]</code> pour présenter du code Python.

Un environnement <code>envconsolepythontex[...]</code> pour présenter une console Python.

![illustr](proflycee-test-codepython.png?raw=true "testcode")

![illustr](proflycee-test-consolepython.png?raw=true "testconsole")
