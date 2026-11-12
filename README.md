# Lab — SCM / Git

Lab en binôme sur Git, en deux parties: la ligne de commande, puis l'intégration dans l'IDE.

## Partie 1 : Git CLI (45 min)

Cette partie peut se finir à la maison.

- [ ] Compléter les niveaux de [Learn Git Branching](https://learngitbranching.js.org)

## Partie 2 : Git avec une intégration IDE

### 1. Prérequis

- [ ] Créer une clé SSH ([doc GitHub](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent))
- [ ] Créer un compte GitHub (si besoin)
- [ ] Ajouter la clé publique au compte GitHub
- [ ] Installer PyCharm CE (si absent)

### 2. Mise en place

- [ ] Créer un repository
- [ ] Récupérer [`awsip.py`](https://github.com/psantus/does-this-ip-belong-to-aws/blob/main/python/awsip.py)

### 3. Évolutions en parallèle

Chaque membre du binôme modifie `awsip.py` sur sa propre branche. Indice: la doc du module [`ipaddress`](https://docs.python.org/3/library/ipaddress.html).

| Membre | Évolution |
|--------|-----------|
| Personne A | Ajouter la première et la dernière IP de la plage |
| Personne B | Ajouter le nombre d'IPs de la plage |

- [ ] Commit et push sur vos branches respectives

### 4. Merge et résolution de conflits

- [ ] Merger l'une des branches sur `main`
- [ ] Résoudre les conflits entre la 2ᵉ branche et `main`, par un rebase ou lors d'un merge

### 5. Feature complexe

- [ ] Développer ensemble une feature décomposée en sous-features. Exemple: trouver le plus petit sous-réseau qui contient N adresses IP.

## Commandes utiles

```bash
git checkout -b feature/ma-branche
git add .
git commit -m "Ajout de ..."
git push -u origin feature/ma-branche
git checkout main && git merge feature/ma-branche
git rebase main
```
