Brillenbar — Kit Nicolas (DNS + GitHub Pages + Sous-domaine)

1) DNS (chez l'hébergeur du domaine brillenbar.org)
   Ajouter l'enregistrement:
     Type: CNAME
     Host: science
     Value: brillenbar.org

2) GitHub Pages (dans le dépôt)
   - Placer les fichiers fournis à la racine du dépôt.
   - Vérifier le fichier 'CNAME' avec le contenu: brillenbar.org
   - Activer Settings → Pages → Deploy from branch (main / root)
   - Custom domain: brillenbar.org
   - Laisser GitHub générer le certificat HTTPS.

3) Structure incluse:
   /index.html                 (portail principal simple)
   /science/index.html         (page de test sous-domaine)
   /science/schema_a3.svg      (schéma A3 diurne)
   /science/schema_a3.png      (schéma A3 diurne, PNG impression)
   /CNAME                      (brillenbar.org)
   /.nojekyll                  (désactive Jekyll)

4) Test
   - Accéder à https://brillenbar.org/
   - Accéder à https://brillenbar.org/science/
   - Accéder à https://science.brillenbar.org/  (doit afficher la même page)

5) Remarques
   - Quand la structure scientifique sera prête, remplacer /science/index.html par le site complet.
   - Zenodo (DOI) se connectera au dépôt après la première release publiée.
