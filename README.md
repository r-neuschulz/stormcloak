# Stormlight Archive Themed Login Field

A custom Keycloak login field inspired by *The Stormlight Archive*, built with [keycloakify](https://docs.keycloakify.dev).


## Screenshot

![Screenshot](Screenshot.png)

## Deploying the theme

### Keycloak 22 – 26 (Quarkus distribution)

1. Grab the latest `keycloak-theme-for-kc-22-to-25.jar` from the [releases](https://github.com/r-neuschulz/stormcloak/releases).  
2. Copy it into your Keycloak installation:  
   ```bash
   cp keycloak-theme-for-kc-22-to-25.jar $KC_HOME/providers/
   ```  
3. Rebuild Keycloak so it picks up the new provider:  
   ```bash
   bin/kc.sh build
   ```  
4. Start (or restart) Keycloak:  
   ```bash
   bin/kc.sh start
   ```  

### Keycloak 15 – 21 (legacy/WildFly distribution)

1. Grab the latest ` keycloak-theme-for-kc-all-other-versions.jar ` from the [releases](https://github.com/r-neuschulz/stormcloak/releases).  
2. Copy it into WildFly’s deployments folder:  
   ```bash
   cp  keycloak-theme-for-kc-all-other-versions.jar $KC_HOME/standalone/deployments/
   ```  
3. Restart Keycloak:  
   ```bash
   bin/standalone.sh
   ```  


## Customizing the theme

For customization strategies and deep dives, see the [keycloakify documentation](https://docs.keycloakify.dev/customization-strategies).


[releases]: https://github.com/your-repo/keycloakify-theme/releases