What is it
===================


This is a maven project intended to be deployed in an instance of Nuxeo 7.10 or 8.1.
This effectively overrides the default theme proposed.

- Language files
- CSS
- Javascript
- XHTML

 
Here's what to do to use it :

1. To start, move in **NUXEO_HOME/nxserver/nuxeo.war/incl/**.
2. Then select the template to override.
3. Create a file with the same name in **/src/main/resources/web/nuxeo.war/incl/**
4. Copy the contents of the template in the newly created file.
5. Make the desired changes
6. Compile the project
7. Deploy

<i class="icon-cog"></i> To compile the project it is necessary to have installed Apache maven.

----------

Deploy
-------------

Moving into the project and run :
```
mvn install
```

Stop Nuxeo

Copy the jar file located in target folder in nuxeo
```
scp -r ./*.jar root@servername:/path/to/nuxeo/nxserver/bundles/
```

Restart Nuxeo
