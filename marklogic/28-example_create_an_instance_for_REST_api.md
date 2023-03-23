# Example: Creating an Instance

## Follow this procedure to create a rest-example database with 3 forests and a rest-example HTTP App Server attached to the database.

* Open power shell

* Create the instance and database by sending a POST request to /rest-apis on port 8002. MarkLogic Server responds with status code 201 (Created). For example:

    ```
    C:\Windows\System32\curl.exe --anyauth --user admin:admin -i -X POST `
    -d'{"rest-api":{"name":"rest-example"}}' `
    -H "Content-type: application/json" `
    "http://3.21.52.79:8002/LATEST/rest-apis"
    ```

* By specifying only the instance name, we request MarkLogic Server to create a database with the same name, including one forest, and to use the next available port above 8002.

* Navigate to the Admin Interface in your browser:

    ```
    http://<your-marklogic-server-host-ip-address>:8001
    ```

* Observe the creation of a database named rest-example with forests named rest-example-1, rest-example-2, and rest-example3; and an HTTP App Server called rest-example attached to this database.

* A modules database is also created for the instance.

* Test the instance by navigating to the following URL in your browser. (Your port number may differ if port 8003 was already in use). When prompted for a username and password, authenticate with a user that has the rest-reader role.

    ```
    http://<your-marklogic-server-host-ip-address>:8003
    ```

* If the instance is properly configured, you will see a short HTML summary of capabilities provided by the instance.