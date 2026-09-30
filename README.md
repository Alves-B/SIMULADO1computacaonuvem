cat> index.html <<'EOF'
<!DOCTYPE html>
<html lang ="pt-BR">
<head>
<meta charset=UTF-8">
<title>Pedidos</title>
</head>
<body>
<h1>Pedidos em funcionamento</h1>
</body>
</html>
EOF




cole aqaui a saida do comando docker ps:
docker ps
CONTAINER ID   IMAGE          COMMAND                  CREATED              STATUS              PORTS                                     NAMES
09bf23138157   nginx:alpine   "/docker-entrypoint.…"   About a minute ago   Up About a minute   0.0.0.0:8084->80/tcp, [::]:8084->80/tcp   pedidos
cole aqui  Resposta do comando  cursl http://localhost:8084
curl http://localhost:8084
<!DOCTYPE html>
<html>
<head>
<title>Welcome to nginx!</title>
<style>
html { color-scheme: light dark; }
body { width: 35em; margin: 0 auto;
font-family: Tahoma, Verdana, Arial, sans-serif; }
</style>
</head>
<body>
<h1>Welcome to nginx!</h1>
<p>If you see this page, nginx is successfully installed and working.
Further configuration is required for the web server, reverse proxy, 
API gateway, load balancer, content cache, or other features.</p>

<p>For online documentation and support please refer to
<a href="https://nginx.org/">nginx.org</a>.<br/>
To engage with the community please visit
<a href="https://community.nginx.org/">community.nginx.org</a>.<br/>
For enterprise grade support, professional services, additional 
security features and capabilities please refer to
<a href="https://f5.com/nginx">f5.com/nginx</a>.</p>

<p><em>Thank you for using nginx.</em></p>
</body>
</html>

3 8084:80 serviu o meu computador e o 80 o computador do servidor
