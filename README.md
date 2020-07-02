# springbootopenapi

Dans une API REST la documentation est importante (springDoc) il est important de simplifier la génération et la maintenance des documents API, basés sur la spécification OpenAPI3.

# Configuration de springdoc-openapi

Srpingdoc-openapi génére automatiquement les documents de spécification OpenAPI3. Il suffit d'ajouter la dépendance adéquate:
"
<dependency>
    <groupId>org.springdoc</groupId>
    <artifactId>springdoc-openapi-ui</artifactId>
    <version>1.2.32</version>
</dependency>
"
Il faut savoir que lors de l'exécution de l'application, les descriptions OpenAPI seront disponible par défaut sur le cemin /V3/api-docs.

# Configuration du projet test

    - un bean (firstname / lastname / email / age / credit number)
    - un controller 

# Configuration du fichier application.properties

  application-description=@project.description@
  
  application-version=@project.version@
  
  logging.level.org.springframework.boot.autoconfigure=ERROR
  
  Les entrées inscritent dans "application.properties" transmettront les informations relatives à la construction de la documentation OpenAPI
  
# Configuration de Springboot application
  
  Nous allons faire une description de notre API en exploitant application.properties
  
# Interface utilisateur Swagger
  
  A ce point il ne reste plus qu'à lancer l'application et se rendre sur :
  
    http://localhost:8080/swagger-ui.html
 
