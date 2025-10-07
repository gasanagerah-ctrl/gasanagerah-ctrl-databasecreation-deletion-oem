# gasanagerah-ctrl-databasecreation-deletion-oem

OVER VIEW OF DATABASE CREATION,DELETION & OEM

TASK

This task went through variuos tasks :

 -Creating new pluggable database in oracle 21
 
 -Creat and delet a PDB
 
 -Configure oracle enteprise manager 

STEPS TAKEN TO COMPLETE THE TASK:

1.we statered by installing oracle 21 

2.second i opened sqlplus and logged as :sqlplus/ as SYSDBA after i inserted the password

3. i created a new PDB as:

CREATE PLUGGABLE DATABASE ga_pdb_28888

ADMIN USER gasana_plsqlauca_28888 IDENTIFIED BY Gasa_na123

4.i opened or listed te db to see if there is no error:

-ALTER PLUGGABLE DATABASE ga_pdb_28888 OPEN

-SHOW PDBS

it displayed the table without any error

5.Another task is to create another PDB and Delete it :

the db was called ga_to_delete_pdb_28888 the syntax:

-CREATE PLUGGABLE DATABASE ga_to_delete_pdb_28888

ADMIN USER gasana_delete_plsqlauca IDENTIFIED  BY Gasa_na123

no issue encoutered so far

-ALTER PLUGGABLE DATABASE ga_to_delete_pdb_28888

-SHOW PDBS

after i closed the PDB so it can be possible to drop:

-ALTER PLUGGABLE DATABASE ga_to_delete_pdb_28888 CLOSE IMMEDIATE

-DROP PLUGGABLE DATABASE ga_to_delete_pdb_28888 INCLUDING DATAFILES

the table was deleted  successfully

6.CONFIGURING ORACLE ENTERPRISE MANAGER

-I opened the browser and went to: https://localhost:5510/em

-i logged in with sys credentials 

NOTES:At the begining of the creating the pluggable DB i set the files to be defaultly saved 
and other problems where slowly solved


 


