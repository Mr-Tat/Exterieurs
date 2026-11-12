# Math'as — Ressources extérieures

Bibliothèque **publique** des liens vers des ressources extérieures à Math'as Connect et de leurs miniatures. Ce dépôt est **séparé** de `Miniatures-Mathas`, réservé aux miniatures des applications.

- [Catalogue des liens externes](catalogue.json)
- [Miniatures](miniatures/)
- [Math'as Connect](https://github.com/Mr-Tat/Mathas-Connect) — affiche les cartes et garde le contrôle des classes, réglages professeur et catégories

## Principe

Un lien = un identifiant stable, un titre, une URL HTTPS, une section et des espaces cibles. La vignette correspondante est stockée dans `miniatures/` lorsque c'est possible. Ce dépôt **ne contient aucun identifiant de classe, nom d'élève, token, score, trophée ou XP**.

La liste JSON est une **source de référence** pour les futurs ajouts ; pour l'instant le HUB lit son catalogue Supabase et dispose d'un secours statique. **Modifier le JSON seul ne publie pas une carte** : chaque ajout est répercuté par une PR Math'as Connect et les permissions du catalogue, avec vérification des classes.

**GitHub Pages n'est pas nécessaire** : les images publiques de ce dépôt peuvent être chargées directement par les clients HTTPS. On pourra mettre en place un site Pages plus tard si un site web de consultation devient utile.

## Premier lien — Padlet jeux

- Adresse : https://padlet.com/julientatas1/jeux-math-6y4b0kwcj5444l83
- Catégorie : **Jeux**, cinq espaces scolaires et l'espace professeur « Toutes » ; accès de test autorisé.
- Miniature : `miniatures/padlet-jeux.webp`, copie autorisée de la miniature déjà utilisée par l'ancien Math'as. L'import initial utilise une action GitHub **ponctuelle**, puis l'image reste autonome dans ce dépôt.
- Pas de connexion automatique au Padlet, ni XP, ni scores Connect.

## Ajouter un autre lien

1. Ajouter un objet validé dans `catalogue.json` avec un identifiant unique, le nom, l'URL, la rubrique et les espaces.
2. Déposer une image WebP légère dans `miniatures/` ; conserver la provenance.
3. Adapter via PR le catalogue de Math'as Connect (données Supabase, et secours statique si adapté), sans modifier les autres jeux.
4. Contrôler l'URL, l'image, la section et les classes réellement publiées.
