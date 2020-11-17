# FReMP - Full Stack App

- FReMP is Flask, ReactJS, MongoDB and Python.

# Setup
1. Install Flask
```
sudo apt-get install python3
sudo apt-get install python3-pip
sudo -H pip3 install flask
flask --version
```
2. Install React
```
sudo apt-get install nodejs
sudo npm install -g yarn
sudo npm install -g npx
yarn --version
npx --version
```
3. Install MongoDB
```
sudo apt-get install mongo
mongo --version
```
# Run
1. Clone
```
git clone https://github.com/greyhub/flask-react-app.git
```
2. Frontend
```
cd flask-react-app/frontend/
yarn start
```
3. Backend
> Ctrl+Shift+T
```
cd ../backend/
python3 app.py
```
Done !

## Handle error
1. Frontend
- Port 3000 is already in use
```
npx kill-port 3000
```

2. Backend
- OSError: [Errno 98] Address already in use Flask error
```
ps -fA | grep python
```
> Check the one with “flask” in the path and note down its PID(process ID).
```
kill -9 pid
```
> e.x. : kill -9 23458
