# Week 1 — App Containerization

tasks:
  - name: aws-cli
    env:
      AWS_CLI_AUTO_PROMPT: on-partial
    init: |
      cd /workspace
      curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
      unzip awscliv2.zip
      sudo ./aws/install
      cd $THEIA_WORKSPACE_ROOT
vscode:
  extensions:
    - 42Crunch.vscode-openapi




gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ aws sts get-caller-id
> aws sts get-caller-identity
{
    "UserId": "XXXXXXXXXXXXV",
    "Account": "xxxxxxxx1695",
    "Arn": "arn:aws:iam::xxxxxxxx1695:user/pd"
}
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ export AWS_ACCOUNT_ID=$(aws sts get-caller-identity --query Account --output text)
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ env AWS_ACCOUNT_ID
env: ‘AWS_ACCOUNT_ID’: No such file or directory
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ env | grep AWS_ACCOUNT_ID
AWS_ACCOUNT_ID=xxxxxxxx1695
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ gp env AWS_ACCOUNT_IS="xxxxxxxx1695"
AWS_ACCOUNT_IS=xxxxxxxx1695
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 


arn:aws:sns:us-east-1:XXXXXXXX1695:Billing-Alert


#---------------------------------------------------------------------------------------------------------------------------------



/api/activities/home

/api/activities/home

export FRONTEND_URL="*"
export BACKEND_URL="*"

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ cd backend
bash: cd: backend: No such file or directory
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ cd backend*
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ pip3 install -r requirements.txt
Requirement already satisfied: flask in /workspace/.pyenv_mirror/user/current/lib/python3.8/site-packages (from -r requirements.txt (line 1)) (2.2.3)
Requirement already satisfied: flask-cors in /workspace/.pyenv_mirror/user/current/lib/python3.8/site-packages (from -r requirements.txt (line 2)) (3.0.10)
Requirement already satisfied: Werkzeug>=2.2.2 in /workspace/.pyenv_mirror/user/current/lib/python3.8/site-packages (from flask->-r requirements.txt (line 1)) (2.2.3)
Requirement already satisfied: itsdangerous>=2.0 in /workspace/.pyenv_mirror/user/current/lib/python3.8/site-packages (from flask->-r requirements.txt (line 1)) (2.1.2)
Requirement already satisfied: importlib-metadata>=3.6.0 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from flask->-r requirements.txt (line 1)) (6.0.0)
Requirement already satisfied: click>=8.0 in /workspace/.pyenv_mirror/user/current/lib/python3.8/site-packages (from flask->-r requirements.txt (line 1)) (8.1.3)
Requirement already satisfied: Jinja2>=3.0 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from flask->-r requirements.txt (line 1)) (3.1.2)
Requirement already satisfied: Six in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from flask-cors->-r requirements.txt (line 2)) (1.16.0)
Requirement already satisfied: zipp>=0.5 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from importlib-metadata>=3.6.0->flask->-r requirements.txt (line 1)) (3.11.0)
Requirement already satisfied: MarkupSafe>=2.0 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from Jinja2>=3.0->flask->-r requirements.txt (line 1)) (2.1.1)

[notice] A new release of pip available: 22.3.1 -> 23.0.1
[notice] To update, run: pip install --upgrade pip
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ export FRONTEND_URL="*"
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ export BACKEND_URL="*"
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ python3 -m flask run --host=0.0.0.0 --port=4567
 * Debug mode: off
WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
 * Running on all addresses (0.0.0.0)
 * Running on http://127.0.0.1:4567
 * Running on http://10.0.5.2:4567
Press CTRL+C to quit
192.168.139.74 - - [13/Mar/2023 04:35:38] "GET / HTTP/1.1" 404 -
192.168.139.74 - - [13/Mar/2023 04:35:38] "GET /favicon.ico HTTP/1.1" 404 -
192.168.139.74 - - [13/Mar/2023 04:36:22] "GET /api/activities/home HTTP/1.1" 200 -
^Cgitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ curl -X GET http://localhost:4567/api/activities/home
[{"created_at":"2023-03-11T00:19:07.170968+00:00","expires_at":"2023-03-18T00:19:07.170968+00:00","handle":"Andrew Brown","likes_count":5,"message":"Cloud is fun!","replies":[{"created_at":"2023-03-11T00:19:07.170968+00:00","handle":"Worf","likes_count":0,"message":"This post has no honor!","replies_count":0,"reply_to_activity_uuid":"68f126b0-1ceb-4a33-88be-d90fa7109eee","reposts_count":0,"uuid":"26e12864-1c26-5c3a-9658-97a10f8fea67"}],"replies_count":1,"reposts_count":0,"uuid":"68f126b0-1ceb-4a33-88be-d90fa7109eee"},{"created_at":"2023-03-06T00:19:07.170968+00:00","expires_at":"2023-03-22T00:19:07.170968+00:00","handle":"Worf","likes":0,"message":"I am out of prune juice","replies":[],"uuid":"66e12864-8c26-4c3a-9658-95a10f8fea67"},{"created_at":"2023-03-12T23:19:07.170968+00:00","expires_at":"2023-03-13T12:19:07.170968+00:00","handle":"Garek","likes":0,"message":"My dear doctor, I am just simple tailor","replies":[],"uuid":"248959df-3079-4947-b847-9e0892d1bab4"}]
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ exit


https://4567-burreetoman-awsbootcamp-4p5m4koar62.ws-us90.gitpod.io/api/activities/home

	
0	
created_at	"2023-03-11T04:36:22.382080+00:00"
expires_at	"2023-03-18T04:36:22.382080+00:00"
handle	"Andrew Brown"
likes_count	5
message	"Cloud is fun!"
replies	
0	
created_at	"2023-03-11T04:36:22.382080+00:00"
handle	"Worf"
likes_count	0
message	"This post has no honor!"
replies_count	0
reply_to_activity_uuid	"68f126b0-1ceb-4a33-88be-d90fa7109eee"
reposts_count	0
uuid	"26e12864-1c26-5c3a-9658-97a10f8fea67"
replies_count	1
reposts_count	0
uuid	"68f126b0-1ceb-4a33-88be-d90fa7109eee"
1	
created_at	"2023-03-06T04:36:22.382080+00:00"
expires_at	"2023-03-22T04:36:22.382080+00:00"
handle	"Worf"
likes	0
message	"I am out of prune juice"
replies	[]
uuid	"66e12864-8c26-4c3a-9658-95a10f8fea67"
2	
created_at	"2023-03-13T03:36:22.382080+00:00"
expires_at	"2023-03-13T16:36:22.382080+00:00"
handle	"Garek"
likes	0
message	"My dear doctor, I am just simple tailor"
replies	[]
uuid	"248959df-3079-4947-b847-9e0892d1bab4"


https://4567-burreetoman-awsbootcamp-4p5m4koar62.ws-us90.gitpod.io

[{"created_at":"2023-03-11T04:36:22.382080+00:00","expires_at":"2023-03-18T04:36:22.382080+00:00","handle":"Andrew Brown","likes_count":5,"message":"Cloud is fun!","replies":[{"created_at":"2023-03-11T04:36:22.382080+00:00","handle":"Worf","likes_count":0,"message":"This post has no honor!","replies_count":0,"reply_to_activity_uuid":"68f126b0-1ceb-4a33-88be-d90fa7109eee","reposts_count":0,"uuid":"26e12864-1c26-5c3a-9658-97a10f8fea67"}],"replies_count":1,"reposts_count":0,"uuid":"68f126b0-1ceb-4a33-88be-d90fa7109eee"},{"created_at":"2023-03-06T04:36:22.382080+00:00","expires_at":"2023-03-22T04:36:22.382080+00:00","handle":"Worf","likes":0,"message":"I am out of prune juice","replies":[],"uuid":"66e12864-8c26-4c3a-9658-95a10f8fea67"},{"created_at":"2023-03-13T03:36:22.382080+00:00","expires_at":"2023-03-13T16:36:22.382080+00:00","handle":"Garek","likes":0,"message":"My dear doctor, I am just simple tailor","replies":[],"uuid":"248959df-3079-4947-b847-9e0892d1bab4"}]


unset FRONTEND_URL
unset BACKEND_URL


gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ docker build -t  backend-flask ./backend-flask
unable to prepare context: path "./backend-flask" not found
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ pwd
/workspace/aws-bootcamp-cruddur-2023/backend-flask
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ ls -l 
total 28
-rw-r--r-- 1 gitpod gitpod 3500 Mar 13 00:30 app.py
-rw-r--r-- 1 gitpod gitpod  261 Mar 13 05:06 Dockerfile
-rw-r--r-- 1 gitpod gitpod 6359 Mar 13 00:30 openapi-3.0.yml
drwxr-xr-x 2 gitpod gitpod   32 Mar 13 00:35 __pycache__
-rw-r--r-- 1 gitpod gitpod  265 Mar 13 00:30 README.md
-rw-r--r-- 1 gitpod gitpod   16 Mar 13 00:30 requirements.txt
drwxr-xr-x 3 gitpod gitpod 4096 Mar 13 00:35 services
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ 
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ 
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ 
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ 
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ cd ..
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ pwd
/workspace/aws-bootcamp-cruddur-2023
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ ls -l 
total 48068
drwxr-xr-x 3 gitpod gitpod       64 Mar 13 00:30 aws
-rw-r--r-- 1 gitpod gitpod 49212093 Mar 13 00:30 awscliv2.zip
drwxr-xr-x 4 gitpod gitpod      175 Mar 13 00:35 backend-flask
drwxr-xr-x 3 gitpod gitpod       20 Mar 13 00:30 _docs
drwxr-xr-x 4 gitpod gitpod      149 Mar 13 00:30 frontend-react-js
drwxr-xr-x 2 gitpod gitpod     4096 Mar 13 00:30 journal
-rw-r--r-- 1 gitpod gitpod      921 Mar 13 00:30 README.md
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker build -t  backend-flask ./backend-flask
Sending build context to Docker daemon   55.3kB
Step 1/8 : FROM python:3.10-slim-buster
3.10-slim-buster: Pulling from library/python
8fd419aca81c: Pull complete 
e53683fb464b: Pull complete 
d63ea5bc79e0: Pull complete 
ab33e3a565e2: Pull complete 
afdf1a7100d3: Pull complete 
Digest: sha256:2425b3b12adf669291256767a3c07257ed4f3f53d26970fd44dc528b824e28dd
Status: Downloaded newer image for python:3.10-slim-buster
 ---> 9ab67b0788d8
Step 2/8 : WORKDIR /backend-flask
 ---> Running in b130e6b1f4b8
Removing intermediate container b130e6b1f4b8
 ---> 036bb2e02d35
Step 3/8 : COPY requirements.txt requirements.txt
 ---> 3d2c7c9e582d
Step 4/8 : RUN pip3 install -r requirements.txt
 ---> Running in 7e89d1597e0e
Collecting flask
  Downloading Flask-2.2.3-py3-none-any.whl (101 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 101.8/101.8 kB 5.0 MB/s eta 0:00:00
Collecting flask-cors
  Downloading Flask_Cors-3.0.10-py2.py3-none-any.whl (14 kB)
Collecting itsdangerous>=2.0
  Downloading itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Collecting Werkzeug>=2.2.2
  Downloading Werkzeug-2.2.3-py3-none-any.whl (233 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 233.6/233.6 kB 21.2 MB/s eta 0:00:00
Collecting Jinja2>=3.0
  Downloading Jinja2-3.1.2-py3-none-any.whl (133 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 133.1/133.1 kB 46.6 MB/s eta 0:00:00
Collecting click>=8.0
  Downloading click-8.1.3-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.6/96.6 kB 39.0 MB/s eta 0:00:00
Collecting Six
  Downloading six-1.16.0-py2.py3-none-any.whl (11 kB)
Collecting MarkupSafe>=2.0
  Downloading MarkupSafe-2.1.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (25 kB)
Installing collected packages: Six, MarkupSafe, itsdangerous, click, Werkzeug, Jinja2, flask, flask-cors
Successfully installed Jinja2-3.1.2 MarkupSafe-2.1.2 Six-1.16.0 Werkzeug-2.2.3 click-8.1.3 flask-2.2.3 flask-cors-3.0.10 itsdangerous-2.1.2
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv

[notice] A new release of pip available: 22.3.1 -> 23.0.1
[notice] To update, run: pip install --upgrade pip
Removing intermediate container 7e89d1597e0e
 ---> c8e219658a90
Step 5/8 : COPY . .
 ---> 8a622a222d68
Step 6/8 : ENV FLASK_ENV=development
 ---> Running in d482ac4a48e2
Removing intermediate container d482ac4a48e2
 ---> 2b833dc90ccf
Step 7/8 : EXPOSE ${PORT}
 ---> Running in 05727549d8fe
Removing intermediate container 05727549d8fe
 ---> c25d64ae7f04
Step 8/8 : CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]
 ---> Running in 316abb9b807f
Removing intermediate container 316abb9b807f
 ---> 59b63722abd0
Successfully built 59b63722abd0
Successfully tagged backend-flask:latest
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker images
REPOSITORY      TAG                IMAGE ID       CREATED          SIZE
backend-flask   latest             59b63722abd0   10 seconds ago   129MB
python          3.10-slim-buster   9ab67b0788d8   11 days ago      118MB
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 


root@5028bd9abb3b:/backend-flask# env
HOSTNAME=5028bd9abb3b
PYTHON_VERSION=3.10.10
PWD=/backend-flask
PYTHON_SETUPTOOLS_VERSION=65.5.1
HOME=/root
LANG=C.UTF-8
GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
TERM=xterm
SHLVL=1
PYTHON_PIP_VERSION=22.3.1
PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
FLASK_ENV=development
_=/usr/bin/env
root@5028bd9abb3b:/backend-flask# 

root@5028bd9abb3b:/backend-flask# env | grep END
root@5028bd9abb3b:/backend-flask# 

docker run --rm -p 4567:4567 -it  --env FRONTEND_URL="*" --env BACKEND_URL="*" backend-flask


gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker run --rm -p 4567:4567 -it --env FRONTEND_URL="*" --env BACKEND_URL="*" backend-flask'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
 * Debug mode: on
WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
 * Running on all addresses (0.0.0.0)
 * Running on http://127.0.0.1:4567
 * Running on http://172.17.0.2:4567
Press CTRL+C to quit
 * Restarting with stat
'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
 * Debugger is active!
 * Debugger PIN: 124-475-716
 *  Executing task: docker exec -it ba6be21bb45051012dc1ce53d82fd997e9ca4c5054df537c757dedac74b2aab1 bash 

# Alternate ways to set up ENV variables.
docker run --rm -p 4567:4567 -it backend-flask
FRONTEND_URL="*" BACKEND_URL="*" docker run --rm -p 4567:4567 -it backend-flask
export FRONTEND_URL="*"
export BACKEND_URL="*"
docker run --rm -p 4567:4567 -it -e FRONTEND_URL='*' -e BACKEND_URL='*' backend-flask
docker run --rm -p 4567:4567 -it  -e FRONTEND_URL -e BACKEND_URL backend-flask
unset FRONTEND_URL="*"
unset BACKEND_URL="*"

# My prefered:
docker run --rm -p 4567:4567 -it  --env FRONTEND_URL="*" --env BACKEND_URL="*" backend-flask

root@ba6be21bb450:/backend-flask# env
FRONTEND_URL=*
HOSTNAME=ba6be21bb450
PYTHON_VERSION=3.10.10
PWD=/backend-flask
PYTHON_SETUPTOOLS_VERSION=65.5.1
HOME=/root
LANG=C.UTF-8
GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
BACKEND_URL=*
TERM=xterm
SHLVL=1
PYTHON_PIP_VERSION=22.3.1
PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
FLASK_ENV=development
_=/usr/bin/env
root@ba6be21bb450:/backend-flask# 


# Execute from Repo level
docker build -t  backend-flask ./backend-flask
# Execute from repo level
docker run --rm -p 4567:4567 -it  --env FRONTEND_URL="*" --env BACKEND_URL="*" backend-flask
# Run docker container in the background (with -d)
docker container run --rm -p 4567:4567 -d backend-flask

# DOCKER COMPOSE FILE:

version: "3.8"
services:
  backend-flask:
    environment:
      FRONTEND_URL: "https://3000-${GITPOD_WORKSPACE_ID}.${GITPOD_WORKSPACE_CLUSTER_HOST}"
      BACKEND_URL: "https://4567-${GITPOD_WORKSPACE_ID}.${GITPOD_WORKSPACE_CLUSTER_HOST}"
    build: ./backend-flask
    ports:
      - "4567:4567"
    volumes:
      - ./backend-flask:/backend-flask
  frontend-react-js:
    environment:
      REACT_APP_BACKEND_URL: "https://4567-${GITPOD_WORKSPACE_ID}.${GITPOD_WORKSPACE_CLUSTER_HOST}"
    build: ./frontend-react-js
    ports:
      - "3000:3000"
    volumes:
      - ./frontend-react-js:/frontend-react-js

# the name flag is a hack to change the default prepend folder
# name when outputting the image names
networks: 
  internal-network:
    driver: bridge
    name: cruddur

# ====================================================
# WEEK-1 TRY-OVER TO UNBREAK NTM INSTALL [03.18.2023]:
# ====================================================

















