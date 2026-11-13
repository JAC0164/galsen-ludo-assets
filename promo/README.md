# Promotion croisée (GalsenPromo)

Les jeux Galsen Games lisent `games.json` pour proposer les autres jeux du studio.
Le plugin et le format sont décrits dans le dépôt `godot-galsen-promo`.

- **Nouveau jeu :** ajouter une entrée à `games.json` et son icône dans `icons/` (PNG 256×256).
- **Jeu sorti :** passer son `enabled` à `true`.
- Garder `id` stable : il sert à la mesure (`promo_game`) et au réglage `galsen_promo/game_id` du jeu.
- Les jeux relisent le flux au plus toutes les 12 h. Le cache de GitHub dure quelques minutes.
