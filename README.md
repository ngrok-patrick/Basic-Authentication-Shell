# Basic-Authentication-Shell
Simple Bash Shell example of performing Basic Authentication

Postman can be used to easily form this request, but if you are curious about how to do it manually, here is a simple example.

```
base64_encoded_credentials=$(echo -n "username:password" | base64)
authorization_header="Authorization: Basic $base64_encoded_credentials"
curl -H "$authorization_header" https://0cd1d75a2b36.ngrok.app

echo "[Basic $base64_encoded_credentials]"
```
Now you know... 😁
