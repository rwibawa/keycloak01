# keycloak01
Exercise and templates to use Keycloak OpenID Connect.

## Modules
* [Microservice Template](https://github.com/rwibawa/keycloak-backend)
* [UI Template with Angular 8](https://github.com/rwibawa/keycloak-ng)

## Docker Setup
```bash
$ docker run -d -p 8088:8080 -p 9990:9990 \
-e KEYCLOAK_USER=admin -e KEYCLOAK_PASSWORD=admin123 \
-e DB_VENDOR=mysql -e DB_ADDR=hh-mysql -e DB_USER=epmsuser -e DB_PASSWORD=epmsmysql \
--network mynetwork --name epms-keycloak \
jboss/keycloak
```

## References
* [https://www.npmjs.com/package/keycloak-angular](https://www.npmjs.com/package/keycloak-angular)
* [https://github.com/mauriciovigolo/keycloak-angular](https://github.com/mauriciovigolo/keycloak-angular)
* [https://medium.com/@sairamkrish/keycloak-integration-part-2-integration-with-angular-frontend-f2716c696a28](https://medium.com/@sairamkrish/keycloak-integration-part-2-integration-with-angular-frontend-f2716c696a28)
* [https://github.com/sairamkrish/keycloak-identity-management-demo](https://github.com/sairamkrish/keycloak-identity-management-demo)
* [https://ultimatesecurity.pro/post/2fa-api/](https://ultimatesecurity.pro/post/2fa-api/)

## Add git submodules
```bash
$ git init
$ vi README.md

$ git submodule add https://github.com/rwibawa/keycloak-backend keycloak-backend
$ git submodule add https://github.com/rwibawa/keycloak-ng keycloak-ng
```
