gwaas-examples
==============

Delivery Type 		Web Service Push / WEBSVC-PUSH
Delivery Format 	Type JSON / JSON

Params

	url				https://yoururl.com/numerex_services/delivery/message
	username	 	username
	password 		password
	auth-type 		basic

curl --user username:password -H "Content-Type: application/json" -X POST http://yoururl.com:8080/numerex_services/delivery/message -d '{"device_name_type":"imei", "device_name":"357820023702392"}'
curl --user username:password -H "Content-Type: application/json" -X POST https://yoururl.com:8080/numerex_services/delivery/message -d '{"device_name_type":"imei", "device_name":"357820023702392"}' -k

openssl genrsa -out privatekey.pem 1024 
openssl req -new -key privatekey.pem -out certrequest.csr 
openssl x509 -req -in certrequest.csr -signkey privatekey.pem -out certificate.pem

express requires "node":">= 0.8.0"