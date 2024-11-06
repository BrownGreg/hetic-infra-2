**Sélectionner les composants AWS dont vous aurez besoin pour déployer votre app**

Pour cette app AWS, j'ai besoin de API Gateway pour gérer les requêtes, dynamoDB pour la DB, S3 pour le stockage, CloudFront pour la distribution, Route 53 pour gérer les DNS, ECR pour stocker les deux images Docker, et CloudWatch pour la gestion des logs et la surveillance de l'app

**Justifier vos choix techniques (il faut bien convaincre vos futurs investisseurs !)**

Avec AWS on peut faire évoluer l'application grâce avec les services API Gateway et DynamoDB qui s'ajustent automatiquement selon la demande et ce, en optimisant les coûts. 
De plus, la force multi-AZ des services DynamoDB, Amazon S3 et API Gateway garantit que l'application reste disponible même en cas de panne. On ne paye que pour ce qu'on utilise, ce qui permet de limiter les dépenses.
Et puis avec des outils comme ECR et CloudFront, on se concentre sur l'application sans se soucier de l'infrastructure.

**Quel service AWS vous avez utilisé pour uploader vos images Docker et les rendre disponibles dans votre projet AWS :**

- Le service Elastic Container Registry (ECR) pour uploader les images Docker afin de rendre disponible le projet dans AWS.

![Schema AWS](schema.png)