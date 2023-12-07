---
title: "Nutri-score: un outil pour mieux manger ?"
permalink: "/title/"
layout: page
---

![screenshot](declinaison-logo-nutriscore.jpg)

# I. Présentation
## 1. Enjeux alimentaires et présentation du Nutri-Score
### a. Pourquoi devrait-on penser à notre alimentation ?
La question de l’alimentation représente un sujet majeur de santé publique. L'alimentation constitue l'une des trois principales causes de morbidité, de mortalité prématurée et de handicap en Europe, selon l’étude Global Burden of Disease (GBD, 2016). De ce fait, la nutrition est un facteur de risque pour plusieurs troubles et maladies chroniques, dont l’obésité, le diabète, les maladies cardiovasculaires, ou certains types de cancers (Ebbeling, 2002 ; Lobstein, 2004). Ce constat est d’autant plus alarmant si l’on considère le fait que 47,3 % de la population française est en surpoids, et 17,0 % est obèse, selon une étude menée à l'initiative de la "Ligue Contre l'Obésité (Fontbonne, 2020). Les causes de cette prévalence de surpoids sont multiples et résultent d’un déséquilibre entre apport et dépense d’énergie. Dans ce contexte, l'étiquetage nutritionnel a émergé de manière progressive en tant que politique alimentaire et préventive majeure, pour faire face à ces nouveaux défis. Ce dernier vise une conscientisation des populations, leur permettant de prendre des décisions de consommation éclairées et plus équilibrées au quotidien. 

### b. Présentation du Nutri-Score :
Adopté en France, en application de la loi de « Modernisation de Notre Système de Santé » du 26 janvier 2016, le Nutri-Score est un système d'étiquetage nutritionnel simplifié et facultatif.

La signalétique du Nutri-Score attribue un score de A (“meilleure qualité nutritionnelle”) à E (“moins bonne qualité nutritionnelle”) aux produits alimentaires. Chaque lettre est accompagnée d'une couleur spécifique, allant du vert au rouge, pour évaluer la qualité nutritionnelle des aliments, en se basant sur une portion de 100 g (Ministère de la Santé et de la Prévention, 2023). Le calcul du score se fonde sur les données fournies par la déclaration nutritionnelle obligatoire associée à chaque produit alimentaire. Le Nutri-Score les classe alors en deux catégories de nutriments : ceux à favoriser, en l’occurrence les fruits, légumes, fibres, protéines, etc., et ceux à limiter, tels que le sucre, acides gras saturés, sel, etc. Le Nutri-Score n’a pas seulement vocation à permettre au consommateur de mieux connaître le profil nutritionnel global des denrées alimentaires. Il constitue une véritable norme qui oriente le choix des consommateurs vers la décision la plus favorable à leur santé, dans un contexte de surcharge informationnelle (Friant-Perrot, 2021).

## 2. Construction du Nutri-Score : comment est fait le calcul? 
Comment est-il précisément calculé, le Nutri-Score ? Comme évoqué précédemment, la classification de la qualité nutritionnelle du produit varie de A à E, avec des couleurs allant du vert foncé au rouge, attribuées en fonction des points obtenus pour 100g. Le calcul se déroule en trois étapes distinctes.

Dans la première étape, des points dits "négatifs" (N), représentant des nutriments dont la consommation est nuisible pour la santé, sont attribués en fonction de la quantité présente dans le produit. Chaque catégorie, comprenant les graisses saturées (g), les sucres simples (g), le sodium/sel (mg) et l'énergie (kJ), est évaluée de 0 à 10 points. Ainsi, le nombre maximal de points négatifs est de 40. Pour la deuxième étape, des points "positifs" (P), favorables à la santé, sont attribués de 0 à 5 pour chacun des éléments suivants : fibres, protéines, teneur en fruits, légumes, certaines huiles et noix (%). Le chiffre maximal possible à atteindre est de 15.

Enfin, lors de la dernière étape, pour obtenir la valeur finale du Nutri-Score, il suffit de soustraire le nombre de points positifs obtenus dans la deuxième étape du nombre de points négatifs de la première étape. Sur une échelle allant de -15 à 40, plus le résultat est bas, meilleure est la qualité nutritionnelle. Une fois le calcul effectué, on associe la valeur nutritionnelle résultante à une lettre en fonction des seuils de classement suivants :
![screenshot](Nutriscore attribution des couleurs.jpg) 

Just fork this [repository](https://github.com/niklasbuschmann/contrast) and adjust the `_config.yml` to use with [Github Pages](https://pages.github.com/) and your page is done.

## Features

 - supports dark mode on macOS Mojave
 - optional sidebar
 - MathJax support
 - no external ressources
 - included archive page
 - supports pagination
 - feed generation
 - responsive
 - syntax highlighting
 - supports comments via [disqus](https://disqus.com/) or [isso](http://posativ.org/isso/)

## Based on

- [Hyde](https://github.com/poole/hyde)
- [Minima](https://github.com/jekyll/minima)
- [Lagrange](https://github.com/LeNPaul/Lagrange)
- [Font Awesome](http://fontawesome.io/)
- [KaTeX](https://katex.org/)
- [Pygments](https://github.com/richleland/pygments-css)

## Installation (jekyll-remote-theme method)

You can use this theme with the `jekyll-remote-theme` plugin. Just create an empty repo, copy over the `index.html` file and add this to your `_config.yml`:

```yaml
remote_theme: niklasbuschmann/contrast@v2.11

plugins:
  - jekyll-remote-theme
```

Note: to enable icons you also need to copy over the `_data` folder.

## Config

Your `_config.yml` could for example look like this:

```yaml
title: "Blog Title"
author: "Blog Author"
description: "My personal blog about ... something"
permalink: /:title/
lang: "en"
excerpt_separator: "\n\n\n"
date_format: "%B %d, %Y"

# Layout

show_excerpts: true        # show article excerpts on the home page
show_frame: true           # adds a gray frame to the site
show_sidebar: false        # show a sidebar instead of the usual header

# Menu

navigation:                # accepts {file, title, url, icon, sidebaricon}
  - {file: "index.html"}
  - {file: "README.md"}

external:                  # shows a footer with social links - for available icons see fontawesome.com/icons
  - {title: Mail, icon: envelope, url: "mailto:niklasbuschmann@users.noreply.github.com"}
  - {title: Github, icon: github, url: "https://github.com/niklasbuschmann/contrast"}
  - {title: Subscribe, icon: rss, url: "/feed.xml"}

comments:
#  disqus_shortname: ""    # see https://disqus.com/
#  isso_domain: ""         # see https://posativ.org/isso/

plugins:
 - jekyll-feed

```

## MathJax

Contrast comes preinstalled with a leightweight alternative to MathJax called [KaTeX](https://katex.org/). To display equations in a post simply set `mathjax: true` in the article's front matter.

## License

[public domain](http://unlicense.org/)

## Screenshots

![screenshot](declinaison-logo-nutriscore.jpg)

![screenshot](https://user-images.githubusercontent.com/4943215/109431832-b6cac080-7a08-11eb-9c5e-a058680c23a1.png)

![screenshot](https://user-images.githubusercontent.com/4943215/73125194-5f0b8b80-3fa4-11ea-805c-8387187503ad.png)

Kaoutar Laklalech - Sofya Davidovich - Raja Madani - Pauline Chatail - Célia Outemzabet - Yeon Hwa Kim
