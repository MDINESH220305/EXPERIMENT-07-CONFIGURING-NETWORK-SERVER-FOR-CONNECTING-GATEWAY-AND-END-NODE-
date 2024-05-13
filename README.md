# NAME:Dinesh.M
# REGNO:212222043002
 ### EXPERIMENT -07 CONFIGURING NETWORK SERVER FOR CONNECTING GATEWAY AND END NODE 
 
## Aim: To  configure  the Network server and end device for traferring data on the network
## Components required: end node stm 32 development kit , dragino LPS8, network server 

## Theory :
When working with sensitive applications or files, saving progress on your local device is a start, but what if you lose access to your device? Network servers address this problem by hosting the files and programs most pertinent to the network and enabling access for consistent, real-time use. 

As a result, personnel or network clients can instantly access important data or tools while also facilitating collaboration between users. Multiple users can make changes to the same program or document for continued development over the course of a project. Via a secure login, remote users can connect to the home network.


![41](https://github.com/MDINESH220305/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/162429215/c97e012b-b0a7-4764-b4fe-fa4bca227e38)

In the above graphic, the circle represents an organization network where a network server facilitates collaboration and file sharing between network clients (devices).

 The role of a network server, then, is to provide users with a set of services and access to resources on the network. These features include:

Permissioned access and log-ins for network users Gateway access to the Internet for an organization Centralized location for network resources  Shared access to devices on the network like a printer or a scanner Hosts multi-user apps like email servers, web applications, or CRM

## Procedure :

 1. login to the network server using login link  https://iot.saveetha.in/
 2. Click on the nework server as shown blow

![42](https://github.com/MDINESH220305/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/162429215/013885a8-e2c2-4533-88a1-bab9088c99a7)

 3. click on the add gateway 

![43](https://github.com/MDINESH220305/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/162429215/bdbde0f1-ea3a-4207-8ffb-a2ccb2b6eb78)


![44](https://github.com/MDINESH220305/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/162429215/6b117983-e40c-4391-99a7-9874a85f3b2f)


![45](https://github.com/MDINESH220305/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/162429215/294e5542-c993-4ce8-818d-311f0956ba23)



4. click on the lora options , lora - frequency plan 
5. click on channel s and create a new channel after which you can add a new end device 

![46](https://github.com/MDINESH220305/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/162429215/5d2eb3ef-23a0-40d4-9f98-01ae487841c0)


6. add the attributesin the end device as  shown below 
![47](https://github.com/MDINESH220305/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/162429215/a732134c-6680-4499-a917-ac5064c53e08)



 
7.using AT commands configure end device in serial port utility
AT Commands to set initially (Mandatory)
 AT+FDR // To do factory data reset
 AT+NJM=1 // To set OTAA mode
 AT+ADR=1 // To enable the ADR
 AT+TDC=600000 // To set the default sampling interval as 10 minutes
(Should not give below 5 minutes)
 AT+CLASS=C // To set class C
 AT+DEUI=XX XX XX XX XX XX XX XX // To set Device EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX // To set APP EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX //
To set APP Key
 ATZ // To take effective action on below settings (As like saving)



## OUTPUT 

![48](https://github.com/MDINESH220305/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/162429215/29ddd7de-0acb-4d39-9f4c-e9ae68a034dd)




## Results: 

  The Network server and end device for traferring data on the network has been accomplished.

