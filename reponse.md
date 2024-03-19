# Réponses aux diverses questions présente dans le travail pratique

## Exercice 1 b)

### Quelles étapes (steps) sont réalisées par cette action ?
- Récupération du code source depuis le référentiel avec actions/checkout@v3.
- Configuration de l'environnement Python avec actions/setup-python@v3.
- Installation des dépendances avec pip.
- Vérification de la qualité du code avec flake8.
- Exécution des tests avec pytest.

### Une étape est définie au minimum par 2 éléments, lesquels sont-ils et à quoi servent-ils ?
- 1) name : C'est le nom de l'étape qui apparaîtra dans le tableau de bord de l'interface GitHub Actions. Il sert à identifier clairement chaque étape du workflow.
- 2) run: C'est l'action à effectuer dans cette étape. Il s'agit généralement d'une commande shell ou d'un script à exécuter. Il est utilisé pour spécifier les actions à entreprendre dans le contexte de cette étape.

### La première étape contient le mot-clé 'with', a quoi sert-il ?
Dans la première étape nommée "Set up Python 3.10", le mot-clé with est utilisé pour spécifier les paramètres pour l'action actions/setup-python@v3. Dans ce cas, il spécifie la version de Python à installer, qui est "3.10".
