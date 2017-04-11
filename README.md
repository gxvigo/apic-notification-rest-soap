# apic-notification-rest-soap

This project implements an IBM API Connect - API Definition application.

It has 1 resource with 1 POST method: 
- sendSms 

The method invoke a SOAP service defined by sms2.wsdl
The assembly make a call to the SOAP endpoint in datapower:8888 and if it fails (ConnectionTimeout) it contact datapower:8889
Both services are implemented (loopback) in a DataPower domain: sms_DataPower-domain.zip
