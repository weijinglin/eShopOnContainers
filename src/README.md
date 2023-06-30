## Deploy Recording

### Use decouple docker-compose file
-   create two docker-compose file and set up. However, the dependency is not being take care in this method, so we need to set up different part in fix turn
-   set up command
    ```
    docker-compose -f docker-compose-pone.yml -f docker-compose.override.one.yml up

    # wait for all container in one had been set up
    
    docker-compose -f docker-compose-ptwo.yml -f docker-compose.override.two.yml up
    ```