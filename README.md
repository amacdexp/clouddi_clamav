# clouddi_clamav 
SAP Cloud DI - Custom operator running clamav 



See SAP Cloud Data intelligence help for creating custom operators, based on dockerfiles 
https://help.sap.com/viewer/1c1341f6911f4da5a35b191b40b426c8/Cloud/en-US/d49a07c5d66c413ab14731adcfc4f6dd.html


NOTE:
You may to needed to first uncomment and build the org.opensuse docker file as the reference base 

##Steps in SAP Cloud DI Modeller 
1) Create dockerfile 
2) give unique tags (identifier) to dockerfile    e.g. clamav 
3) create operator (linked to tags) e.g.  clamav 
    Change AWS key and Secret, pass in parameters 
    Change AWS bucket details 
4) Create graph 



#Test
In terminal type in file name to scan 
~Aprox 20 seconds later results or san are sent to wiretap 

