# Matières premières · Flashcards

Application de révision type Anki pour le cours **GENV003-1 — Conception durable & économie circulaire** (ULiège). Tout tient dans un seul fichier HTML : aucune installation, aucun serveur obligatoire.

## Contenu

- **748 cartes** question / réponse
- **3 parties** : Pirard, Léonard, Courard
- Thèmes variés (technologie, GHG Protocol, matériaux, etc.) regroupés par section

## Lancer l’application

1. Ouvrir `index.html` dans un navigateur récent (Chrome, Firefox, Safari, Edge).
2. Ou double-cliquer sur le fichier dans le Finder / l’explorateur de fichiers.

**Astuce :** si les accents s’affichent mal, recharger la page après mise à jour du fichier. Le document déclare bien l’encodage UTF-8 (`<meta charset="UTF-8">`).

Pour un serveur local optionnel :

```bash
cd carte_mem_thib
python3 -m http.server 8080
```

Puis ouvrir [http://localhost:8080/](http://localhost:8080/).

## Utilisation

### Tableau de bord

- Statistiques : nouvelles cartes, à réviser, maîtrisées
- Lancer une session sur l’ensemble du deck ou sur un chapitre
- Réinitialiser tous les progrès (action irréversible)

### Session d’étude

1. Lire la question sur la carte.
2. **Espace** ou clic sur « Afficher la réponse ».
3. Noter la carte :

| Bouton      | Touche | Effet (prochaine révision) |
|------------|--------|----------------------------|
| À revoir    | `1`    | < 1 min                    |
| Difficile  | `2`    | 1 heure                    |
| Correct    | `3`    | 1 jour                     |
| Facile     | `4`    | 2 jours                    |

Les cartes « dues » réapparaissent selon ces intervalles (répétition espacée simplifiée).

### Parcourir

- Recherche dans les questions, réponses et sections
- Filtre par chapitre
- Aperçu question / réponse sans lancer une session

## Sauvegarde des progrès

La progression (cartes vues, dates de révision) est enregistrée **dans le navigateur** sous la clé `genv003_progress`. Elle reste disponible tant que vous ouvrez le fichier depuis le même navigateur et que les données du site ne sont pas effacées.

## Structure du projet

```
carte_mem_thib/
├── README.md
└── index.html   # application complète (HTML, CSS, JS, données)
```

## Prérequis

- Navigateur moderne avec JavaScript activé
- Connexion internet utile uniquement pour charger les polices Google Fonts (Fraunces, Inter, JetBrains Mono)

## Licence

Contenu pédagogique lié au cours GENV003-1. Usage personnel pour la révision.
