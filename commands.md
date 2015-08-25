#commands.md

$> docker build -t docker-training:1.0 .
$> docker run --name mysql -e MYSQL_ROOT_PASSWORD=secret -e MYSQL_DATABASE=homestead -e MYSQL_USER=homestead -e MYSQL_PASSWORD=secret -d mysql:5.6
$> docker run --name worldapi --link mysql:mysql -p 80:80 -v /home/mgiorda/docker-final-project/worldapi:/opt/www/worldapi -d docker-training:1.0