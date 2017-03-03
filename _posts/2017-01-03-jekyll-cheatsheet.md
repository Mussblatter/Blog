---
layout: post
title:  "Jekyll cheatsheet"
date:   2017-01-03 18:00
categories: Cheatsheet
---

# Création d'un post

Pour créer un nouveau post sur Jekyll : **YYYY-DD-MM-title.md**

~~~
---
layout: post
title:  "Jekyll cheatsheet"
date:   2017-01-03 18:00
categories: Categorie1 Categorie2
---
~~~

# Utilisation de Git

Pour cloner un repo :

`git clone repo_url.git`

Pour récupérer du repo :

`git pull`

Pour envoyer au repo :

 `git commit -a -m "message"`

 `git push origin`

Pour enregistrer le pseudo et mot de passe :

`git config credential.helper cache`

Pour qu’il ne s’en souvienne que pour une durée limitée (temps en secondes) :

`git config credential.helper 'cache --timeout=3600'`

Et si vous souhaitez qu’il oublie le login/mot de passe avant le délai d’expiration, il suffit de tuer le démon avec :

`git credential-cache exit`

# Markdown syntaxe

### Images

`![Title](url)`

### Liens

`[Title](url)`
