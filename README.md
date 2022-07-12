# sf5-microservices-project

## Prerequisites
In order to run this project, first start Vault server in dev mode using following command

      vault server -dev
    
When Vault server is up and running, update environment variable for vault token and add key value pairs as secret from order-service and than from product-service directory

      vault kv put secret/order-service @order-service.json
      vault kv put secret/product-service @product-service.json
      vault kv put secret/inventory-service @inventory-service-credentials.json
    
 Locate to bin directory of Keycloak installation and run command

      standalone.bat -Djboss.http.port=8180
    
 Access to Authorization Server Configuration - Keycloak

      localhost:8180
        





    
