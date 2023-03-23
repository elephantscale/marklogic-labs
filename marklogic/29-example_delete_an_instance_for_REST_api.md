# Delete an instance

## The following example removes the RESTstop instance, including the content and modules databases, and the forests attached to the databases:

* Open power shell

* Run belwo command

    ```
    C:\Windows\System32\curl.exe -X DELETE --anyauth admin:admin -i `
  'http://3.21.52.79:8002/LATEST/rest-apis/RESTstop?include=content&include=modules'
    ```

* If the instance name is not unique across groups, use the group request parameter to differentiate the target instance.

* The following URL requests removal of the instance of RESTstop in the stage group:

    ```
    hC:\Windows\System32\curl.exe -X DELETE --anyauth --user admin:admin -i `
  "http://3.21.52.79:8002/LATEST/rest-apis/RESTstop?group=stage"
    ```
