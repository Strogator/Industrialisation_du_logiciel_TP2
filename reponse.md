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

## Exercice 2 a)

### Sur l’onglet Summary d’une analyse de code, SonarCloud fournit 4 indicateurs. Quels sont-ils et quelles sont leurs utilités ?

- 1 Bugs : Cet indicateur montre le nombre de bogues identifiés dans le code source.

- 2 Vulnerabilities : Il indique le nombre de vulnérabilités de sécurité détectées dans le code. Celles-ci peuvent créer des failles permettant aux attaquants de compromettre la sécurité du système.

- 3 Code Smells : Ou mauvaise pratique en français, ce sont des parties du code qui fonctionnent correctement, mais qui peuvent être améliorées en termes de lisibilité, de maintenabilité ou de performances.

- 4 Coverage : C'est le pourcentage de code source couvert par des tests unitaires. Plus celle-ci est élevée, plus le code est testé et moins il y a de risques de régressions ou d'erreur. 

### À quoi sert l’indicateur Quality Gate ?

L'indicateur Quality Gate est un seuil de qualité défini pour le projet. Il permet de déterminer si le code respecte les critères de qualité définis par l'équipe de développement. Si le code ne respecte pas ces critères, le Quality Gate échoue et le code ne peut pas être validé pour la production. Cela permet de garantir un niveau de qualité constant et d'éviter l'introduction de bogues ou de vulnérabilités dans le code.