Generate Token:
curl --request POST \
--url http://localhost:8088/api/auth/login \
--header 'Content-Type: application/json' \
--header 'User-Agent: insomnia/11.4.0' \
--data ' {
"username": "admin",
"password": "admin123"
}'

---------------------------------------------------------------------
Access secure API:
curl --request GET \
--url 'http://localhost:8088/api/secure/hello?=&=' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJhZG1pbiIsImlhdCI6MTc1NDEwOTgxOCwiZXhwIjoxNzU0MTk2MjE4fQ.agEQd3cgIfQXpf0K8PCRanvSiTs1klCdLbIb4fqro0s' \
--header 'Content-Type: application/json' \
--header 'User-Agent: insomnia/11.4.0' \
--data ' '
--------------------------------------------------------------------------------------
cmd:
curl -H "Authorization: Bearer <your_token>" http://localhost:8088/api/secure/hello


