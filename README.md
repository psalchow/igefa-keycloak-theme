# Keycloak Theme for igefa

### How to use

1. Checkout Repository
2. Build theme with `./gradlew build`
3. Test the theme by starting Keycloak docker container with `docker compose up -d`
4. Browse to http://localhost:8080/ and login with `admin:admin`
5. In the Realm settings -> Themes select the `igefa` Theme for Login
6. Logout and checkout the Login-Screen

## Production use

1. Build theme with `./gradlew build`
2. Build a new docker image that is based on `quay.io/keycloak/keycloak:22.0.3` and copy `build/libs/igefa-keycloak-theme.jar` to `/opt/keycloak/providers` within the image