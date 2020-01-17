<a href="www.keepizi.com"><img src="https://www.keepizi.com/wp-content/uploads/2018/08/Logo-Keepizi_violet_mobile.png" title="Keepizi" alt="Keepizi"></a>

***Exercice de mise en ligne d'un projet AJX via Git***

# AJOUT D'ARTICLES FAVORIS
> Des articles apparaissent pour l'utilisateur. AU clic, l'article est ajouté aux favoris via la SESSION. Lors du déclic, l'icône favoris disparait et l'article est enlevé de la SESSION.

> Tech: AJAX, Javascript, PHP

**N'oubliez pas de ...**
- Si vous souhaitez lier à une base de données, créez votre fichier d'initialisation dans le dossier inc.
- Le sarticles apparaissent en dur dans notre index, veuillez les remplacer par les vôtres.

> Ajout de notre GIF [![LES FAVORIS SELON LES GOONIES](https://media.giphy.com/media/UWKGHQa8ze32U/giphy.gif)]())

## Table des matières 

- [Explication](#explication)
- [Remerciment](#remerciement)

```PHP
// Traitement du retrait des favoris
            if(isset($_POST["a"]) && $_POST["a"] == "remove")
            {
                foreach ($_SESSION['favorites'] as $key => $value)
                {
                  if($id == $value)
                  {
                    unset($_SESSION['favorites'][$key]);
                  }
                }
            }
```
- Pour retirer les favoris de ma SESSION, je regarde bien que l'action demandée est un "remove";
- Je fais concorder le $id envoyé en POST avc les valeurs enregistrées en SESSION.

---
# Remerciements
---

A tous les étudiants !

[![Veuillez visiter notre site](https://media.giphy.com/media/cJ7gVV0QL9RPG/giphy.gif)](https://www.keepizi.com/)