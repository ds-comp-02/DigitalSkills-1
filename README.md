DigitalSkills

install docker mongodb-clients nodejs npm ns-common git

docker run --name mongo --net fabmedical -p 27017:27017 -d mongo:4.0

cd ~/content-init
npm install

nodejs server.js

mongo
use contentdbs
db.speakers.find()
db.sessions.find()
quit()

cd ../content-api
npm install

nodejs ./server.js &

curl localhost:3001/speakers

cd ../content-web
npm install
ng build

pub ip add to app.js

node app.js &

curl localhost:3000
