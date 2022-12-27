# jbossTestDS
Tiny app to test a datasource

standalone.xml

Except

Set Java Property import.file with path to import_data.sql

<connection-url>jdbc:h2:mem:test;DB_CLOSE_DELAY=-1;DB_CLOSE_ON_EXIT=FALSE;INIT=RUNSCRIPT FROM '${import.file:/absolutePath/import_data.sql}';</connection-url>
