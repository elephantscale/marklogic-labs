# Connect to webdav from windows

### Steps to Connect to a Web Folder in Windows Explorer:

* Double-click the My Network Places icon on your desktop

* In My Network Places, double-click the Add Network Places icon.

* In the Add Network Place Wizard, enter your WebDAV server address and port number. For example, if you have a WebDAV server running on port 10103 on a machine named ec2-user@3.21.52.79, enter the following URL:

    ```shell
        http://ec2-user@3.21.52.79:10103/
    ```

* Click Next

* If prompted, enter your username and password for the WebDAV server

* Enter a name for the network place and click finish

* You can now use this folder like other Windows folders to drag and drop documents, rename documents, and so on. When you drag and drop a file into a WebDAV folder connected to a MarkLogic Server WebDAV server, you will actually load that document into the database
