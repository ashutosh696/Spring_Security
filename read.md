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
curl --request GET \
--url http://localhost:8088/api/secure/hello \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJhZG1pbiIsImlhdCI6MTc1NDExMjI5OSwiZXhwIjoxNzU0MTk4Njk5fQ.hJbRuxt21qCxdce5N0wQbUV5qvUDGIkH-pBse1RgclA' \
--header 'Content-Type: application/json' \
--header 'User-Agent: insomnia/11.4.0' \
--data ' '
--------------------------------------------------------------------------------------
cmd:
curl -H "Authorization: Bearer <your_token>" http://localhost:8088/api/secure/hello


