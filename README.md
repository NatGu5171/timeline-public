# Timeline publique

Version publique en lecture seule de la frise chronologique Ecole de guerre.

Fichiers servis par GitHub Pages :

- `index.html`
- `timeline-public.html`
- `ecole_de_guerre_timeline_v4.json`

## Fonctionnalités

- Visualisation chronologique des événements, périodes et mandats politiques (1943–1975)
- Filtres par type, catégorie, thème, acteurs et période
- Recherche plein texte
- Panneau de détail par événement
- Interface responsive : desktop, tablette (769–1024 px) et mobile (≤ 768 px)

## Responsive mobile

Sur écran mobile (≤ 768 px) :

- Le panneau de filtres est masqué par défaut et s'ouvre en overlay plein-écran via le bouton **☰ Filtres**
- Les filtres sont validés et l'overlay fermé via le bouton **Valider**
- Le layout multi-colonnes (mandats / événements / périodes) est remplacé par une colonne unique chronologique
- Les tailles de police, marges et paddings sont réduits (~85 % des valeurs desktop)
- Le header est sticky et toutes les cibles tactiles font au minimum 44 px

## Publier une mise à jour

Le dépôt est configuré avec une clé SSH Deploy Key (accès en écriture). Claude Code peut pousser directement sans intervention manuelle.

```bash
cd "Documents/Claude Code/Timeline/public"

# Vérifier les changements
git status
git diff

# Committer et pousser
git add <fichier>
git commit -m "Description du changement"
git push origin main
```

GitHub Pages se redéploie automatiquement après chaque push sur `main` (délai ~30 secondes).
