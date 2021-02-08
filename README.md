# mockapi
mockapi para pruebas
yum update -y
curl -sL https://rpm.nodesource.com/setup_10.x | sudo bash -
sudo yum install nodejs -y
node --version
npm --version

npm install -g json-server
json-server --watch db.json
json-server --host 192.168.1.212 db.json

firewall-cmd --permanent --zone=public --add-port=3000/tcp
firewall-cmd --reload

wget http://192.168.1.212:3000/burgers
