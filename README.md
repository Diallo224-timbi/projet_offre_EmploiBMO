# Tableau de bord des offres d’emploi et des projets de recrutement

Ce projet est un tableau de bord interactif pour explorer les offres d’emploi du secteur social et médico-social en France et les projets de recrutement issus de l’enquête BMO de France Travail.

## Fonctionnalités

- **Offres d’emploi (France Travail)** : statistiques par région, commune, département et métier, filtres et exploration des offres.
- **Projets de recrutement (BMO)** : vues régionale et départementale, graphiques par métier et évolution annuelle avec prévisions.
- Info-bulles interactives sur les graphiques.

La page BMO s’affiche par défaut. Les deux vues sont accessibles depuis les boutons de navigation en haut de page.

## Ouvrir le tableau de bord

1. Téléchargez ou clonez le dossier du projet.
2. Ouvrez `rendu.html` dans un navigateur récent (Chrome, Edge ou Firefox).
3. Une connexion Internet est nécessaire pour charger D3.js depuis jsDelivr.

Si l’ouverture directe du fichier ne fonctionne pas, démarrez un serveur web local depuis ce dossier, puis ouvrez l’adresse indiquée par le serveur. Par exemple, avec Python :

```powershell
python -m http.server 8000
```

Ouvrez ensuite <http://localhost:8000/rendu.html>.

## Fichiers

| Fichier | Rôle |
| --- | --- |
| `rendu.html` | Page du tableau de bord, styles, interactions, données intégrées et graphiques D3.js. |
| `offre-descriptions.js` | Descriptions complètes associées aux offres; chargé par la page. |
| `Logo-lariis-couleur.png` | Logo LARiiS affiché dans la page. |
| `HÉTIS_Logo_couleur.png` | Logo HÉTIS affiché dans la page. |

Conservez ces fichiers dans le même dossier afin que les scripts et logos soient trouvés.

## Technologies et données

- HTML, CSS et JavaScript.
- [D3.js v7](https://d3js.org/), chargé depuis le CDN jsDelivr.
- Les données BMO et les données de synthèse des offres sont intégrées à `rendu.html`.
- Les descriptions complètes sont chargées depuis `offre-descriptions.js`.
- Les prévisions présentées pour 2026–2028 sont calculées à partir de la série 2017–2025. Elles constituent une extrapolation et non des résultats observés.

Les données BMO sont attribuées à l’enquête BMO de France Travail. Pour toute publication ou réutilisation, vérifier les sources, périodes et conditions d’utilisation des données d’offres et des descriptions.

## Utilisation de l’intelligence artificielle

Ce projet a été conçu avec l’assistance de GitHub Copilot et de Claude, principalement pour l’aide au développement, la structuration du code et la rédaction de certaines formulations.

Les outils d’IA ont été utilisés sous la supervision d’un développeur humain : les modifications, données, calculs, interfaces et formulations sont vérifiés, corrigés et validés par une main humaine avant utilisation.
