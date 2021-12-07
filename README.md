# sample-php-mysql-containerized-app
git clone https://github.com/gkrishnans/sample-php-mysql-containerized-app.git</br>
docker network create sample-php-mysql-containerized-network</br>
cd mysql</br>
docker build -t mysql-image .</br>
docker run --name mysql -d --network sample-php-mysql-containerized-network --rm mysql-image</br>
cd ..</br>
cd apache</br>
docker build -t apache-image . </br>
docker run --name apache -d --network sample-php-mysql-containerized-network -p 8888:80 --rm apache-image</br></br>



