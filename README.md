# Kart BI

Un jeu de course 3D qui tourne directement dans Power BI.

J'étais parti sur une idée un peu bête : voir si on pouvait faire rouler des karts dans un rapport. Ça marche. Quatre karts, trois circuits, trois tours contre des bots, avec dérapages, objets et tout le reste.

C'est une parodie, gratuite et non commerciale. Elle n'a aucun lien avec Nintendo.

## Ce que contient ce dépôt

- `KartBI.pbiviz` : le visuel Power BI (version 1.0.0.4)
- `Karts.csv` : la table de départ avec les karts et leurs stats

Je ne publie pas le code source. Le visuel est fourni tel quel.

## Installer

Il vous faut Power BI Desktop (Windows).

1. **Importez la table.** *Accueil → Obtenir les données → Texte/CSV*, puis choisissez `Karts.csv`.
2. **Importez le visuel.** Dans le volet *Visualisations*, cliquez sur les trois points `…`, puis *Importer un visuel à partir d'un fichier*, et prenez `KartBI.pbiviz`.
3. **Ajoutez-le à une page** et agrandissez-le (900 × 500 pixels, c'est confortable).
4. **Glissez les colonnes** de la table `Karts` dans les champs du visuel : Kart, Couleur, Vitesse, Accélération, Maniabilité. Si Power BI écrit « Somme de… » sur un champ, cliquez sur sa flèche et choisissez *Ne pas résumer*.
5. **Cliquez dans le visuel** pour qu'il reçoive le clavier, puis sur *Départ*.

Si vous mettez le visuel à jour, supprimez l'ancien avant d'importer le nouveau, puis remettez les champs.

## Jouer

| Action | Touche |
|---|---|
| Accélérer / freiner | Flèches haut et bas, ou Z et S |
| Tourner | Flèches gauche et droite, ou Q et D |
| Déraper | Maj ou Espace |
| Utiliser un objet | E ou X |
| Se replacer sur la piste | R |
| Pause | P ou Échap |

Pour déraper, tournez en gardant Maj enfoncé. Plus la glissade dure, plus les étincelles changent de couleur (bleu, orange, rose). Relâchez Maj pour partir en turbo.

Sur la piste, les cubes bleus donnent un objet au hasard : un turbo, une banane à poser derrière soi, ou une carapace qui vise le kart devant vous. Les pastilles jaunes et orange donnent un coup de turbo.

Le bouton *Bots* du menu règle la difficulté (Facile, Normal, Difficile).

## Vos propres karts

`Karts.csv` est une table comme une autre. Ajoutez des lignes, changez les couleurs (au format `#e63946`) ou les notes.

Les trois notes (Vitesse, Accélération, Maniabilité) vont de 1 à 10. Au-delà, elles sont ramenées à 10. Un segment sur la colonne `Kart` permet de filtrer les karts proposés au départ.

Vos meilleurs tours sont enregistrés dans le rapport, par circuit et par kart.

## À savoir

- Power BI n'est pas un moteur de jeu. Il n'y a pas de vrai temps réel, et la fluidité dépend de votre machine.
- Le visuel est personnalisé et non certifié. Certaines organisations bloquent ce type de fichier.
- Si le clavier ne répond plus, cliquez de nouveau dans le visuel. Échap peut aussi déclencher des raccourcis de Power BI : utilisez P dans ce cas.
- Je l'ai pensé pour Power BI Desktop. Je ne l'ai pas testé sur le service en ligne.

## Crédits

Fait par ATTUOMAN PRINCE JOSIAS KOFFI.
