# mesher-nginx-example
This example shows you how to use mesher

## Quick Start
***Clone the code***
```sh
git clone https://github.com/thandayuthapani/mesher-nginx-example.git
```
***Run Script***
```sh
bash -x config_env.sh
```
***Run the docker compose file***
```sh
docker-compose up
```
***Check for containers***
Check whether four containers are up and running when running the following command
```sh
docker ps
```
***Set the proxy***
```sh
export http_proxy=0.0.0.0:30101 #mesher-consumer has it's port exposed to machine's port of 30101
```
***curl nginx***

curl nginx and check whether response is coming or not
```sh
curl http://nginx

<!DOCTYPE html>
<html>
<head>
<title>Welcome to nginx!</title>
<style>
    body {
        width: 35em;
        margin: 0 auto;
        font-family: Tahoma, Verdana, Arial, sans-serif;
    }
</style>
</head>
<body>
<h1>Welcome to nginx!</h1>
<p>If you see this page, the nginx web server is successfully installed and
working. Further configuration is required.</p>

<p>For online documentation and support please refer to
<a href="http://nginx.org/">nginx.org</a>.<br/>
Commercial support is available at
<a href="http://nginx.com/">nginx.com</a>.</p>

<p><em>Thank you for using nginx.</em></p>
</body>
</html>

```
