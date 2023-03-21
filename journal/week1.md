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

# CONFIGURE DOCKER FILE AND BUILD CONTAINER/IMAGE:
# ------------------------------------------------

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker build -t  backend-flask ./backend-flask
Sending build context to Docker daemon  33.79kB
Step 1/8 : FROM python:3.10-slim-buster
3.10-slim-buster: Pulling from library/python
8fd419aca81c: Pull complete 
e53683fb464b: Pull complete 
ee020a7334e9: Pull complete 
85e535e79006: Pull complete 
2cf037f769d8: Pull complete 
Digest: sha256:520537d39498addbb048e847381108f52659330c0e13438cccb45311395cc870
Status: Downloaded newer image for python:3.10-slim-buster
 ---> 83773ada8884
Step 2/8 : WORKDIR /backend-flask
 ---> Running in f4c7244cd618
Removing intermediate container f4c7244cd618
 ---> 21e8dbf799cb
Step 3/8 : COPY requirements.txt requirements.txt
 ---> 0daadf6e5aa3
Step 4/8 : RUN pip3 install -r requirements.txt
 ---> Running in e3dde7485b48
Collecting flask
  Downloading Flask-2.2.3-py3-none-any.whl (101 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 101.8/101.8 kB 6.5 MB/s eta 0:00:00
Collecting flask-cors
  Downloading Flask_Cors-3.0.10-py2.py3-none-any.whl (14 kB)
Collecting itsdangerous>=2.0
  Downloading itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Collecting Werkzeug>=2.2.2
  Downloading Werkzeug-2.2.3-py3-none-any.whl (233 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 233.6/233.6 kB 27.4 MB/s eta 0:00:00
Collecting click>=8.0
  Downloading click-8.1.3-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.6/96.6 kB 41.6 MB/s eta 0:00:00
Collecting Jinja2>=3.0
  Downloading Jinja2-3.1.2-py3-none-any.whl (133 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 133.1/133.1 kB 49.9 MB/s eta 0:00:00
Collecting Six
  Downloading six-1.16.0-py2.py3-none-any.whl (11 kB)
Collecting MarkupSafe>=2.0
  Downloading MarkupSafe-2.1.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (25 kB)
Installing collected packages: Six, MarkupSafe, itsdangerous, click, Werkzeug, Jinja2, flask, flask-cors
Successfully installed Jinja2-3.1.2 MarkupSafe-2.1.2 Six-1.16.0 Werkzeug-2.2.3 click-8.1.3 flask-2.2.3 flask-cors-3.0.10 itsdangerous-2.1.2
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv

[notice] A new release of pip available: 22.3.1 -> 23.0.1
[notice] To update, run: pip install --upgrade pip
Removing intermediate container e3dde7485b48
 ---> defeaf8e4896
Step 5/8 : COPY . .
 ---> 2a5771aaf470
Step 6/8 : ENV FLASK_ENV=development
 ---> Running in 7611b920893e
Removing intermediate container 7611b920893e
 ---> e53a9fd77d85
Step 7/8 : EXPOSE ${PORT}
 ---> Running in bdcafd3041b0
Removing intermediate container bdcafd3041b0
 ---> 96e4e4b89af4
Step 8/8 : CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]
 ---> Running in a8b9cc7bfa62
Removing intermediate container a8b9cc7bfa62
 ---> 4938dada5ebc
Successfully built 4938dada5ebc
Successfully tagged backend-flask:latest
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 

# ADD URL COMPLETION TO ACTIVE URL FOR BACKEND-FLASK:
# ---------------------------------------------------

/api/activities/home

# RESULTING JSON OUTPUT FROM FUNCITONING BACKEND-FLASK:
# -----------------------------------------------------

[
  {
    "created_at": "2023-03-16T18:30:06.244103+00:00",
    "expires_at": "2023-03-23T18:30:06.244103+00:00",
    "handle": "Andrew Brown",
    "likes_count": 5,
    "message": "Cloud is fun!",
    "replies": [
      {
        "created_at": "2023-03-16T18:30:06.244103+00:00",
        "handle": "Worf",
        "likes_count": 0,
        "message": "This post has no honor!",
        "replies_count": 0,
        "reply_to_activity_uuid": "68f126b0-1ceb-4a33-88be-d90fa7109eee",
        "reposts_count": 0,
        "uuid": "26e12864-1c26-5c3a-9658-97a10f8fea67"
      }
    ],
    "replies_count": 1,
    "reposts_count": 0,
    "uuid": "68f126b0-1ceb-4a33-88be-d90fa7109eee"
  },
  {
    "created_at": "2023-03-11T18:30:06.244103+00:00",
    "expires_at": "2023-03-27T18:30:06.244103+00:00",
    "handle": "Worf",
    "likes": 0,
    "message": "I am out of prune juice",
    "replies": [],
    "uuid": "66e12864-8c26-4c3a-9658-95a10f8fea67"
  },
  {
    "created_at": "2023-03-18T17:30:06.244103+00:00",
    "expires_at": "2023-03-19T06:30:06.244103+00:00",
    "handle": "Garek",
    "likes": 0,
    "message": "My dear doctor, I am just simple tailor",
    "replies": [],
    "uuid": "248959df-3079-4947-b847-9e0892d1bab4"
  }
]

# RUN CONAINTER IN THE BACKGROUND, ASSIGN CONTAINER-ID TO VARIABLE
# ----------------------------------------------------------------

CONTAINER_ID=$(docker run --rm -p 4567:4567 -d backend-flask)

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ CONTAINER_ID=$(docker run --rm -p 4567:4567 -d backend-flask)
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker ps
CONTAINER ID   IMAGE           COMMAND                  CREATED          STATUS          PORTS                                       NAMES
c17f34619288   backend-flask   "python3 -m flask ru…"   21 seconds ago   Up 19 seconds   0.0.0.0:4567->4567/tcp, :::4567->4567/tcp   blissful_joliot
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker images
REPOSITORY      TAG                IMAGE ID       CREATED          SIZE
backend-flask   latest             4938dada5ebc   12 minutes ago   130MB
python          3.10-slim-buster   83773ada8884   40 hours ago     118MB
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 

# CURL TEST SERVER
# ----------------
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ curl -X GET http://localhost:4567/api/activities/home -H "Accept: application/json" -H "Content-Type: application/json"
<!doctype html>
<html lang=en>
  <head>
    <title>TypeError: argument of type 'NoneType' is not iterable
 // Werkzeug Debugger</title>
    <link rel="stylesheet" href="?__debugger__=yes&amp;cmd=resource&amp;f=style.css">
    <link rel="shortcut icon"
        href="?__debugger__=yes&amp;cmd=resource&amp;f=console.png">
    <script src="?__debugger__=yes&amp;cmd=resource&amp;f=debugger.js"></script>
    <script>
      var CONSOLE_MODE = false,
          EVALEX = true,
          EVALEX_TRUSTED = false,
          SECRET = "IABiWD81qnn3jr9SJOqn";
    </script>
  </head>
  <body style="background-color: #fff">
    <div class="debugger">
<h1>TypeError</h1>
<div class="detail">
  <p class="errormsg">TypeError: argument of type &#39;NoneType&#39; is not iterable
</p>
</div>
<h2 class="traceback">Traceback <em>(most recent call last)</em></h2>
<div class="traceback">
  <h3></h3>
  <ul><li><div class="frame" id="frame-140169385192000">
  <h4>File <cite class="filename">"/usr/local/lib/python3.10/site-packages/flask/app.py"</cite>,
      line <em class="line">2551</em>,
      in <code class="function">__call__</code></h4>
  <div class="source "><pre class="line before"><span class="ws">    </span>def __call__(self, environ: dict, start_response: t.Callable) -&gt; t.Any:</pre>
<pre class="line before"><span class="ws">        </span>&#34;&#34;&#34;The WSGI server calls the Flask application object as the</pre>
<pre class="line before"><span class="ws">        </span>WSGI application. This calls :meth:`wsgi_app`, which can be</pre>
<pre class="line before"><span class="ws">        </span>wrapped to apply middleware.</pre>
<pre class="line before"><span class="ws">        </span>&#34;&#34;&#34;</pre>
<pre class="line current"><span class="ws">        </span>return self.wsgi_app(environ, start_response)</pre></div>
</div>

<li><div class="frame" id="frame-140169385737264">
  <h4>File <cite class="filename">"/usr/local/lib/python3.10/site-packages/flask/app.py"</cite>,
      line <em class="line">2531</em>,
      in <code class="function">wsgi_app</code></h4>
  <div class="source "><pre class="line before"><span class="ws">            </span>try:</pre>
<pre class="line before"><span class="ws">                </span>ctx.push()</pre>
<pre class="line before"><span class="ws">                </span>response = self.full_dispatch_request()</pre>
<pre class="line before"><span class="ws">            </span>except Exception as e:</pre>
<pre class="line before"><span class="ws">                </span>error = e</pre>
<pre class="line current"><span class="ws">                </span>response = self.handle_exception(e)</pre>
<pre class="line after"><span class="ws">            </span>except:  # noqa: B001</pre>
<pre class="line after"><span class="ws">                </span>error = sys.exc_info()[1]</pre>
<pre class="line after"><span class="ws">                </span>raise</pre>
<pre class="line after"><span class="ws">            </span>return response(environ, start_response)</pre>
<pre class="line after"><span class="ws">        </span>finally:</pre></div>
</div>

<li><div class="frame" id="frame-140169385737376">
  <h4>File <cite class="filename">"/usr/local/lib/python3.10/site-packages/flask_cors/extension.py"</cite>,
      line <em class="line">165</em>,
      in <code class="function">wrapped_function</code></h4>
  <div class="source "><pre class="line before"><span class="ws">        </span># Wrap exception handlers with cross_origin</pre>
<pre class="line before"><span class="ws">        </span># These error handlers will still respect the behavior of the route</pre>
<pre class="line before"><span class="ws">        </span>if options.get(&#39;intercept_exceptions&#39;, True):</pre>
<pre class="line before"><span class="ws">            </span>def _after_request_decorator(f):</pre>
<pre class="line before"><span class="ws">                </span>def wrapped_function(*args, **kwargs):</pre>
<pre class="line current"><span class="ws">                    </span>return cors_after_request(app.make_response(f(*args, **kwargs)))</pre>
<pre class="line after"><span class="ws">                </span>return wrapped_function</pre>
<pre class="line after"><span class="ws"></span> </pre>
<pre class="line after"><span class="ws">            </span>if hasattr(app, &#39;handle_exception&#39;):</pre>
<pre class="line after"><span class="ws">                </span>app.handle_exception = _after_request_decorator(</pre>
<pre class="line after"><span class="ws">                    </span>app.handle_exception)</pre></div>
</div>

<li><div class="frame" id="frame-140169385805968">
  <h4>File <cite class="filename">"/usr/local/lib/python3.10/site-packages/flask/app.py"</cite>,
      line <em class="line">2528</em>,
      in <code class="function">wsgi_app</code></h4>
  <div class="source "><pre class="line before"><span class="ws">        </span>ctx = self.request_context(environ)</pre>
<pre class="line before"><span class="ws">        </span>error: t.Optional[BaseException] = None</pre>
<pre class="line before"><span class="ws">        </span>try:</pre>
<pre class="line before"><span class="ws">            </span>try:</pre>
<pre class="line before"><span class="ws">                </span>ctx.push()</pre>
<pre class="line current"><span class="ws">                </span>response = self.full_dispatch_request()</pre>
<pre class="line after"><span class="ws">            </span>except Exception as e:</pre>
<pre class="line after"><span class="ws">                </span>error = e</pre>
<pre class="line after"><span class="ws">                </span>response = self.handle_exception(e)</pre>
<pre class="line after"><span class="ws">            </span>except:  # noqa: B001</pre>
<pre class="line after"><span class="ws">                </span>error = sys.exc_info()[1]</pre></div>
</div>

<li><div class="frame" id="frame-140169385806080">
  <h4>File <cite class="filename">"/usr/local/lib/python3.10/site-packages/flask/app.py"</cite>,
      line <em class="line">1826</em>,
      in <code class="function">full_dispatch_request</code></h4>
  <div class="source "><pre class="line before"><span class="ws">            </span>rv = self.preprocess_request()</pre>
<pre class="line before"><span class="ws">            </span>if rv is None:</pre>
<pre class="line before"><span class="ws">                </span>rv = self.dispatch_request()</pre>
<pre class="line before"><span class="ws">        </span>except Exception as e:</pre>
<pre class="line before"><span class="ws">            </span>rv = self.handle_user_exception(e)</pre>
<pre class="line current"><span class="ws">        </span>return self.finalize_request(rv)</pre>
<pre class="line after"><span class="ws"></span> </pre>
<pre class="line after"><span class="ws">    </span>def finalize_request(</pre>
<pre class="line after"><span class="ws">        </span>self,</pre>
<pre class="line after"><span class="ws">        </span>rv: t.Union[ft.ResponseReturnValue, HTTPException],</pre>
<pre class="line after"><span class="ws">        </span>from_error_handler: bool = False,</pre></div>
</div>

<li><div class="frame" id="frame-140169385806192">
  <h4>File <cite class="filename">"/usr/local/lib/python3.10/site-packages/flask/app.py"</cite>,
      line <em class="line">1847</em>,
      in <code class="function">finalize_request</code></h4>
  <div class="source "><pre class="line before"><span class="ws"></span> </pre>
<pre class="line before"><span class="ws">        </span>:internal:</pre>
<pre class="line before"><span class="ws">        </span>&#34;&#34;&#34;</pre>
<pre class="line before"><span class="ws">        </span>response = self.make_response(rv)</pre>
<pre class="line before"><span class="ws">        </span>try:</pre>
<pre class="line current"><span class="ws">            </span>response = self.process_response(response)</pre>
<pre class="line after"><span class="ws">            </span>request_finished.send(self, response=response)</pre>
<pre class="line after"><span class="ws">        </span>except Exception:</pre>
<pre class="line after"><span class="ws">            </span>if not from_error_handler:</pre>
<pre class="line after"><span class="ws">                </span>raise</pre>
<pre class="line after"><span class="ws">            </span>self.logger.exception(</pre></div>
</div>

<li><div class="frame" id="frame-140169385806304">
  <h4>File <cite class="filename">"/usr/local/lib/python3.10/site-packages/flask/app.py"</cite>,
      line <em class="line">2340</em>,
      in <code class="function">process_response</code></h4>
  <div class="source "><pre class="line before"><span class="ws">            </span>response = self.ensure_sync(func)(response)</pre>
<pre class="line before"><span class="ws"></span> </pre>
<pre class="line before"><span class="ws">        </span>for name in chain(request.blueprints, (None,)):</pre>
<pre class="line before"><span class="ws">            </span>if name in self.after_request_funcs:</pre>
<pre class="line before"><span class="ws">                </span>for func in reversed(self.after_request_funcs[name]):</pre>
<pre class="line current"><span class="ws">                    </span>response = self.ensure_sync(func)(response)</pre>
<pre class="line after"><span class="ws"></span> </pre>
<pre class="line after"><span class="ws">        </span>if not self.session_interface.is_null_session(ctx.session):</pre>
<pre class="line after"><span class="ws">            </span>self.session_interface.save_session(self, ctx.session, response)</pre>
<pre class="line after"><span class="ws"></span> </pre>
<pre class="line after"><span class="ws">        </span>return response</pre></div>
</div>

<li><div class="frame" id="frame-140169385806416">
  <h4>File <cite class="filename">"/usr/local/lib/python3.10/site-packages/flask_cors/extension.py"</cite>,
      line <em class="line">185</em>,
      in <code class="function">cors_after_request</code></h4>
  <div class="source "><pre class="line before"><span class="ws">        </span>normalized_path = unquote_plus(request.path)</pre>
<pre class="line before"><span class="ws">        </span>for res_regex, res_options in resources:</pre>
<pre class="line before"><span class="ws">            </span>if try_match(normalized_path, res_regex):</pre>
<pre class="line before"><span class="ws">                </span>LOG.debug(&#34;Request to &#39;%s&#39; matches CORS resource &#39;%s&#39;. Using options: %s&#34;,</pre>
<pre class="line before"><span class="ws">                      </span>request.path, get_regexp_pattern(res_regex), res_options)</pre>
<pre class="line current"><span class="ws">                </span>set_cors_headers(resp, res_options)</pre>
<pre class="line after"><span class="ws">                </span>break</pre>
<pre class="line after"><span class="ws">        </span>else:</pre>
<pre class="line after"><span class="ws">            </span>LOG.debug(&#39;No CORS rule matches&#39;)</pre>
<pre class="line after"><span class="ws">        </span>return resp</pre>
<pre class="line after"><span class="ws">    </span>return cors_after_request</pre></div>
</div>

<li><div class="frame" id="frame-140169385806528">
  <h4>File <cite class="filename">"/usr/local/lib/python3.10/site-packages/flask_cors/core.py"</cite>,
      line <em class="line">245</em>,
      in <code class="function">set_cors_headers</code></h4>
  <div class="source "><pre class="line before"><span class="ws">    </span># headers allow repeated values.</pre>
<pre class="line before"><span class="ws">    </span>if (not isinstance(resp.headers, Headers)</pre>
<pre class="line before"><span class="ws">           </span>and not isinstance(resp.headers, MultiDict)):</pre>
<pre class="line before"><span class="ws">        </span>resp.headers = MultiDict(resp.headers)</pre>
<pre class="line before"><span class="ws"></span> </pre>
<pre class="line current"><span class="ws">    </span>headers_to_set = get_cors_headers(options, request.headers, request.method)</pre>
<pre class="line after"><span class="ws"></span> </pre>
<pre class="line after"><span class="ws">    </span>LOG.debug(&#39;Settings CORS headers: %s&#39;, str(headers_to_set))</pre>
<pre class="line after"><span class="ws"></span> </pre>
<pre class="line after"><span class="ws">    </span>for k, v in headers_to_set.items():</pre>
<pre class="line after"><span class="ws">        </span>resp.headers.add(k, v)</pre></div>
</div>

<li><div class="frame" id="frame-140169385811904">
  <h4>File <cite class="filename">"/usr/local/lib/python3.10/site-packages/flask_cors/core.py"</cite>,
      line <em class="line">177</em>,
      in <code class="function">get_cors_headers</code></h4>
  <div class="source "><pre class="line before"><span class="ws"></span> </pre>
<pre class="line before"><span class="ws">    </span>return None</pre>
<pre class="line before"><span class="ws"></span> </pre>
<pre class="line before"><span class="ws"></span> </pre>
<pre class="line before"><span class="ws"></span>def get_cors_headers(options, request_headers, request_method):</pre>
<pre class="line current"><span class="ws">    </span>origins_to_set = get_cors_origins(options, request_headers.get(&#39;Origin&#39;))</pre>
<pre class="line after"><span class="ws">    </span>headers = MultiDict()</pre>
<pre class="line after"><span class="ws"></span> </pre>
<pre class="line after"><span class="ws">    </span>if not origins_to_set:  # CORS is not enabled for this route</pre>
<pre class="line after"><span class="ws">        </span>return headers</pre>
<pre class="line after"><span class="ws"></span> </pre></div>
</div>

<li><div class="frame" id="frame-140169385812016">
  <h4>File <cite class="filename">"/usr/local/lib/python3.10/site-packages/flask_cors/core.py"</cite>,
      line <em class="line">153</em>,
      in <code class="function">get_cors_origins</code></h4>
  <div class="source "><pre class="line before"><span class="ws">                </span>return None</pre>
<pre class="line before"><span class="ws">            </span>else:</pre>
<pre class="line before"><span class="ws">                </span>return [&#39;*&#39;]</pre>
<pre class="line before"><span class="ws">        </span>else:</pre>
<pre class="line before"><span class="ws">            </span># Return all origins that are not regexes.</pre>
<pre class="line current"><span class="ws">            </span>return sorted([o for o in origins if not probably_regex(o)])</pre>
<pre class="line after"><span class="ws"></span> </pre>
<pre class="line after"><span class="ws">    </span># Terminate these steps, return the original request untouched.</pre>
<pre class="line after"><span class="ws">    </span>else:</pre>
<pre class="line after"><span class="ws">        </span>LOG.debug(&#34;The request did not contain an &#39;Origin&#39; header. This means the browser or client did not request CORS, ensure the Origin Header is set.&#34;)</pre>
<pre class="line after"><span class="ws">        </span>return None</pre></div>
</div>

<li><div class="frame" id="frame-140169385812128">
  <h4>File <cite class="filename">"/usr/local/lib/python3.10/site-packages/flask_cors/core.py"</cite>,
      line <em class="line">153</em>,
      in <code class="function">&lt;listcomp&gt;</code></h4>
  <div class="source "><pre class="line before"><span class="ws">                </span>return None</pre>
<pre class="line before"><span class="ws">            </span>else:</pre>
<pre class="line before"><span class="ws">                </span>return [&#39;*&#39;]</pre>
<pre class="line before"><span class="ws">        </span>else:</pre>
<pre class="line before"><span class="ws">            </span># Return all origins that are not regexes.</pre>
<pre class="line current"><span class="ws">            </span>return sorted([o for o in origins if not probably_regex(o)])</pre>
<pre class="line after"><span class="ws"></span> </pre>
<pre class="line after"><span class="ws">    </span># Terminate these steps, return the original request untouched.</pre>
<pre class="line after"><span class="ws">    </span>else:</pre>
<pre class="line after"><span class="ws">        </span>LOG.debug(&#34;The request did not contain an &#39;Origin&#39; header. This means the browser or client did not request CORS, ensure the Origin Header is set.&#34;)</pre>
<pre class="line after"><span class="ws">        </span>return None</pre></div>
</div>

<li><div class="frame" id="frame-140169385812240">
  <h4>File <cite class="filename">"/usr/local/lib/python3.10/site-packages/flask_cors/core.py"</cite>,
      line <em class="line">261</em>,
      in <code class="function">probably_regex</code></h4>
  <div class="source "><pre class="line before"><span class="ws">        </span>return True</pre>
<pre class="line before"><span class="ws">    </span>else:</pre>
<pre class="line before"><span class="ws">        </span>common_regex_chars = [&#39;*&#39;, &#39;\\&#39;, &#39;]&#39;, &#39;?&#39;, &#39;$&#39;, &#39;^&#39;, &#39;[&#39;, &#39;]&#39;, &#39;(&#39;, &#39;)&#39;]</pre>
<pre class="line before"><span class="ws">        </span># Use common characters used in regular expressions as a proxy</pre>
<pre class="line before"><span class="ws">        </span># for if this string is in fact a regex.</pre>
<pre class="line current"><span class="ws">        </span>return any((c in maybe_regex for c in common_regex_chars))</pre>
<pre class="line after"><span class="ws"></span> </pre>
<pre class="line after"><span class="ws"></span>def re_fix(reg):</pre>
<pre class="line after"><span class="ws">    </span>&#34;&#34;&#34;</pre>
<pre class="line after"><span class="ws">        </span>Replace the invalid regex r&#39;*&#39; with the valid, wildcard regex r&#39;/.*&#39; to</pre>
<pre class="line after"><span class="ws">        </span>enable the CORS app extension to have a more user friendly api.</pre></div>
</div>

<li><div class="frame" id="frame-140169385812352">
  <h4>File <cite class="filename">"/usr/local/lib/python3.10/site-packages/flask_cors/core.py"</cite>,
      line <em class="line">261</em>,
      in <code class="function">&lt;genexpr&gt;</code></h4>
  <div class="source "><pre class="line before"><span class="ws">        </span>return True</pre>
<pre class="line before"><span class="ws">    </span>else:</pre>
<pre class="line before"><span class="ws">        </span>common_regex_chars = [&#39;*&#39;, &#39;\\&#39;, &#39;]&#39;, &#39;?&#39;, &#39;$&#39;, &#39;^&#39;, &#39;[&#39;, &#39;]&#39;, &#39;(&#39;, &#39;)&#39;]</pre>
<pre class="line before"><span class="ws">        </span># Use common characters used in regular expressions as a proxy</pre>
<pre class="line before"><span class="ws">        </span># for if this string is in fact a regex.</pre>
<pre class="line current"><span class="ws">        </span>return any((c in maybe_regex for c in common_regex_chars))</pre>
<pre class="line after"><span class="ws"></span> </pre>
<pre class="line after"><span class="ws"></span>def re_fix(reg):</pre>
<pre class="line after"><span class="ws">    </span>&#34;&#34;&#34;</pre>
<pre class="line after"><span class="ws">        </span>Replace the invalid regex r&#39;*&#39; with the valid, wildcard regex r&#39;/.*&#39; to</pre>
<pre class="line after"><span class="ws">        </span>enable the CORS app extension to have a more user friendly api.</pre></div>
</div>
</ul>
  <blockquote>TypeError: argument of type &#39;NoneType&#39; is not iterable
</blockquote>
</div>

<div class="plain">
    <p>
      This is the Copy/Paste friendly version of the traceback.
    </p>
    <textarea cols="50" rows="10" name="code" readonly>Traceback (most recent call last):
  File &#34;/usr/local/lib/python3.10/site-packages/flask/app.py&#34;, line 2551, in __call__
    return self.wsgi_app(environ, start_response)
  File &#34;/usr/local/lib/python3.10/site-packages/flask/app.py&#34;, line 2531, in wsgi_app
    response = self.handle_exception(e)
  File &#34;/usr/local/lib/python3.10/site-packages/flask_cors/extension.py&#34;, line 165, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
  File &#34;/usr/local/lib/python3.10/site-packages/flask/app.py&#34;, line 2528, in wsgi_app
    response = self.full_dispatch_request()
  File &#34;/usr/local/lib/python3.10/site-packages/flask/app.py&#34;, line 1826, in full_dispatch_request
    return self.finalize_request(rv)
  File &#34;/usr/local/lib/python3.10/site-packages/flask/app.py&#34;, line 1847, in finalize_request
    response = self.process_response(response)
  File &#34;/usr/local/lib/python3.10/site-packages/flask/app.py&#34;, line 2340, in process_response
    response = self.ensure_sync(func)(response)
  File &#34;/usr/local/lib/python3.10/site-packages/flask_cors/extension.py&#34;, line 185, in cors_after_request
    set_cors_headers(resp, res_options)
  File &#34;/usr/local/lib/python3.10/site-packages/flask_cors/core.py&#34;, line 245, in set_cors_headers
    headers_to_set = get_cors_headers(options, request.headers, request.method)
  File &#34;/usr/local/lib/python3.10/site-packages/flask_cors/core.py&#34;, line 177, in get_cors_headers
    origins_to_set = get_cors_origins(options, request_headers.get(&#39;Origin&#39;))
  File &#34;/usr/local/lib/python3.10/site-packages/flask_cors/core.py&#34;, line 153, in get_cors_origins
    return sorted([o for o in origins if not probably_regex(o)])
  File &#34;/usr/local/lib/python3.10/site-packages/flask_cors/core.py&#34;, line 153, in &lt;listcomp&gt;
    return sorted([o for o in origins if not probably_regex(o)])
  File &#34;/usr/local/lib/python3.10/site-packages/flask_cors/core.py&#34;, line 261, in probably_regex
    return any((c in maybe_regex for c in common_regex_chars))
  File &#34;/usr/local/lib/python3.10/site-packages/flask_cors/core.py&#34;, line 261, in &lt;genexpr&gt;
    return any((c in maybe_regex for c in common_regex_chars))
TypeError: argument of type &#39;NoneType&#39; is not iterable
</textarea>
</div>
<div class="explanation">
  The debugger caught an exception in your WSGI application.  You can now
  look at the traceback which led to the error.  <span class="nojavascript">
  If you enable JavaScript you can also use additional features such as code
  execution (if the evalex feature is enabled), automatic pasting of the
  exceptions and much more.</span>
</div>
      <div class="footer">
        Brought to you by <strong class="arthur">DON'T PANIC</strong>, your
        friendly Werkzeug powered traceback interpreter.
      </div>
    </div>

    <div class="pin-prompt">
      <div class="inner">
        <h3>Console Locked</h3>
        <p>
          The console is locked and needs to be unlocked by entering the PIN.
          You can find the PIN printed out on the standard output of your
          shell that runs the server.
        <form>
          <p>PIN:
            <input type=text name=pin size=14>
            <input type=submit name=btn value="Confirm Pin">
        </form>
      </div>
    </div>
  </body>
</html>

<!--

Traceback (most recent call last):
  File "/usr/local/lib/python3.10/site-packages/flask/app.py", line 2551, in __call__
    return self.wsgi_app(environ, start_response)
  File "/usr/local/lib/python3.10/site-packages/flask/app.py", line 2531, in wsgi_app
    response = self.handle_exception(e)
  File "/usr/local/lib/python3.10/site-packages/flask_cors/extension.py", line 165, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
  File "/usr/local/lib/python3.10/site-packages/flask/app.py", line 2528, in wsgi_app
    response = self.full_dispatch_request()
  File "/usr/local/lib/python3.10/site-packages/flask/app.py", line 1826, in full_dispatch_request
    return self.finalize_request(rv)
  File "/usr/local/lib/python3.10/site-packages/flask/app.py", line 1847, in finalize_request
    response = self.process_response(response)
  File "/usr/local/lib/python3.10/site-packages/flask/app.py", line 2340, in process_response
    response = self.ensure_sync(func)(response)
  File "/usr/local/lib/python3.10/site-packages/flask_cors/extension.py", line 185, in cors_after_request
    set_cors_headers(resp, res_options)
  File "/usr/local/lib/python3.10/site-packages/flask_cors/core.py", line 245, in set_cors_headers
    headers_to_set = get_cors_headers(options, request.headers, request.method)
  File "/usr/local/lib/python3.10/site-packages/flask_cors/core.py", line 177, in get_cors_headers
    origins_to_set = get_cors_origins(options, request_headers.get('Origin'))
  File "/usr/local/lib/python3.10/site-packages/flask_cors/core.py", line 153, in get_cors_origins
    return sorted([o for o in origins if not probably_regex(o)])
  File "/usr/local/lib/python3.10/site-packages/flask_cors/core.py", line 153, in <listcomp>
    return sorted([o for o in origins if not probably_regex(o)])
  File "/usr/local/lib/python3.10/site-packages/flask_cors/core.py", line 261, in probably_regex
    return any((c in maybe_regex for c in common_regex_chars))
  File "/usr/local/lib/python3.10/site-packages/flask_cors/core.py", line 261, in <genexpr>
    return any((c in maybe_regex for c in common_regex_chars))
TypeError: argument of type 'NoneType' is not iterable


-->
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 

# -------------------------------------------------------------
# CHECK CONTAINER LOGS WITH CONTAINER RUNNING IN THE BACKGROUND
# -------------------------------------------------------------

# THIS RUN OF BANCEND_FLAKS FAILED BECAUSE THE ENVIRONMENT VARIABLES WERE NOT SET PRIOR TO RUNNING THE CONTAINER
# --------------------------------------------------------------------------------------------------------------
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ CONTAINER_ID=$(docker run --rm -p 4567:4567 -d backend-flask)
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker logs $CONTAINER_ID -f
'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
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
 * Debugger PIN: 124-475-803
192.168.105.142 - - [18/Mar/2023 18:49:51] "GET / HTTP/1.1" 404 -
192.168.105.142 - - [18/Mar/2023 18:50:32] "GET /api/activities/home HTTP/1.1" 500 -
Traceback (most recent call last):
  File "/usr/local/lib/python3.10/site-packages/flask/app.py", line 2551, in __call__
    return self.wsgi_app(environ, start_response)
  File "/usr/local/lib/python3.10/site-packages/flask/app.py", line 2531, in wsgi_app
    response = self.handle_exception(e)
  File "/usr/local/lib/python3.10/site-packages/flask_cors/extension.py", line 165, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
  File "/usr/local/lib/python3.10/site-packages/flask/app.py", line 2528, in wsgi_app
    response = self.full_dispatch_request()
  File "/usr/local/lib/python3.10/site-packages/flask/app.py", line 1826, in full_dispatch_request
    return self.finalize_request(rv)
  File "/usr/local/lib/python3.10/site-packages/flask/app.py", line 1847, in finalize_request
    response = self.process_response(response)
  File "/usr/local/lib/python3.10/site-packages/flask/app.py", line 2340, in process_response
    response = self.ensure_sync(func)(response)
  File "/usr/local/lib/python3.10/site-packages/flask_cors/extension.py", line 185, in cors_after_request
    set_cors_headers(resp, res_options)
  File "/usr/local/lib/python3.10/site-packages/flask_cors/core.py", line 245, in set_cors_headers
    headers_to_set = get_cors_headers(options, request.headers, request.method)
  File "/usr/local/lib/python3.10/site-packages/flask_cors/core.py", line 177, in get_cors_headers
    origins_to_set = get_cors_origins(options, request_headers.get('Origin'))
  File "/usr/local/lib/python3.10/site-packages/flask_cors/core.py", line 153, in get_cors_origins
    return sorted([o for o in origins if not probably_regex(o)])
  File "/usr/local/lib/python3.10/site-packages/flask_cors/core.py", line 153, in <listcomp>
    return sorted([o for o in origins if not probably_regex(o)])
  File "/usr/local/lib/python3.10/site-packages/flask_cors/core.py", line 261, in probably_regex
    return any((c in maybe_regex for c in common_regex_chars))
  File "/usr/local/lib/python3.10/site-packages/flask_cors/core.py", line 261, in <genexpr>
    return any((c in maybe_regex for c in common_regex_chars))
TypeError: argument of type 'NoneType' is not iterable
192.168.105.142 - - [18/Mar/2023 18:50:32] "GET /api/activities/home?__debugger__=yes&cmd=resource&f=debugger.js HTTP/1.1" 200 -
192.168.105.142 - - [18/Mar/2023 18:50:32] "GET /api/activities/home?__debugger__=yes&cmd=resource&f=style.css HTTP/1.1" 200 -
192.168.105.142 - - [18/Mar/2023 18:50:32] "GET /api/activities/home?__debugger__=yes&cmd=resource&f=console.png HTTP/1.1" 200 -
^C
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 

# SUCCESSFUL ATTEMPT TO RUN BACKEND_FLASK IN BACKGROUND AND GRAB LOGS AND CURL THE URL
# ------------------------------------------------------------------------------------

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ env | grep BAACKEND
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ env | grep BACKEND
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker run --rm -p 4567:4567 -it  --env FRONTEND_URL="*" --env BACKEND_URL="*" backend-flask^C

# ENV VARS INJECTED INTO ENV AT EXECUATION OF BACK_FLASK CONTAINER.
#   ERROR GENERATED BECAUSE CONTAINER WAS ALREADY RUNNING USING THE SAME PORT 4567

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ CONTAINER_ID=$(docker run --rm -p 4567:4567 --env FRONTEND_URL="*" --env BACKEND_URL="*" -d backend-flask)docker: Error response from daemon: driver failed programming external connectivity on endpoint competent_brattain (d42974405ba91c5e1de8bae5d9172bca5f9eec1c2e574ea0c642868c60650b0e): Bind for 0.0.0.0:4567 failed: port is already allocated.
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 

# BELOW IS A SUCCESSFUL RUN OF THE CONTAINER WITH THE ENV VARS INJECTED PRIOR
# DOCKER LOG OF THIS CONTAINER FOLLOWS

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ CONTAINER_ID=$(docker run --rm -p 4567:4567 --env FRONTEND_URL="*" --env BACKEND_URL="*" -d backend-flask)gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker logs $CONTAINER_ID -f
'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
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
 * Debugger PIN: 124-475-803
192.168.195.11 - - [18/Mar/2023 19:02:44] "GET / HTTP/1.1" 404 -
192.168.195.11 - - [18/Mar/2023 19:02:44] "GET /favicon.ico HTTP/1.1" 404 -
192.168.195.11 - - [18/Mar/2023 19:05:08] "GET /api/activities/home HTTP/1.1" 200 -
^C

# DOCKER IMAGE AND CONTAINER STATES

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker ps
CONTAINER ID   IMAGE           COMMAND                  CREATED         STATUS         PORTS                                       NAMES
9fc075296429   backend-flask   "python3 -m flask ru…"   3 minutes ago   Up 3 minutes   0.0.0.0:4567->4567/tcp, :::4567->4567/tcp   intelligent_shockley
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker images
REPOSITORY      TAG                IMAGE ID       CREATED          SIZE
backend-flask   latest             4938dada5ebc   41 minutes ago   130MB
python          3.10-slim-buster   83773ada8884   40 hours ago     118MB

# DOCKER LOG 

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker logs $CONTAINER_ID -f
'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
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
 * Debugger PIN: 124-475-803
192.168.195.11 - - [18/Mar/2023 19:02:44] "GET / HTTP/1.1" 404 -
192.168.195.11 - - [18/Mar/2023 19:02:44] "GET /favicon.ico HTTP/1.1" 404 -
192.168.195.11 - - [18/Mar/2023 19:05:08] "GET /api/activities/home HTTP/1.1" 200 -
^C

# CURL AGAINST RUNNING BACKEND_FLASK CONTAINER

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ curl -X GET http://localhost:4567/api/activities/home -H "Accept: application/json" -H "Content-Type: application/json"
[
  {
    "created_at": "2023-03-16T19:06:35.848761+00:00",
    "expires_at": "2023-03-23T19:06:35.848761+00:00",
    "handle": "Andrew Brown",
    "likes_count": 5,
    "message": "Cloud is fun!",
    "replies": [
      {
        "created_at": "2023-03-16T19:06:35.848761+00:00",
        "handle": "Worf",
        "likes_count": 0,
        "message": "This post has no honor!",
        "replies_count": 0,
        "reply_to_activity_uuid": "68f126b0-1ceb-4a33-88be-d90fa7109eee",
        "reposts_count": 0,
        "uuid": "26e12864-1c26-5c3a-9658-97a10f8fea67"
      }
    ],
    "replies_count": 1,
    "reposts_count": 0,
    "uuid": "68f126b0-1ceb-4a33-88be-d90fa7109eee"
  },
  {
    "created_at": "2023-03-11T19:06:35.848761+00:00",
    "expires_at": "2023-03-27T19:06:35.848761+00:00",
    "handle": "Worf",
    "likes": 0,
    "message": "I am out of prune juice",
    "replies": [],
    "uuid": "66e12864-8c26-4c3a-9658-95a10f8fea67"
  },
  {
    "created_at": "2023-03-18T18:06:35.848761+00:00",
    "expires_at": "2023-03-19T07:06:35.848761+00:00",
    "handle": "Garek",
    "likes": 0,
    "message": "My dear doctor, I am just simple tailor",
    "replies": [],
    "uuid": "248959df-3079-4947-b847-9e0892d1bab4"
  }
]

# FULL DOCKER LOG OF ALL CONTAINER ACTIVITIES FROM ABOVE.
# CONTAINER IS TERMINATED THROUGH USE OF DOCKER EXTENSION AT END OF THIS SECTION (NOTHING TO SEE REALLY)

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker logs $CONTAINER_ID -f
'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
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
 * Debugger PIN: 124-475-803
192.168.195.11 - - [18/Mar/2023 19:02:44] "GET / HTTP/1.1" 404 -
192.168.195.11 - - [18/Mar/2023 19:02:44] "GET /favicon.ico HTTP/1.1" 404 -
192.168.195.11 - - [18/Mar/2023 19:05:08] "GET /api/activities/home HTTP/1.1" 200 -
172.17.0.1 - - [18/Mar/2023 19:06:35] "GET /api/activities/home HTTP/1.1" 200 -
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 

# GAINING ACCESS TO THE INSIDE DOCKER CONTAINER
#     Access was gained using the Docker extension Container tool right-click on container, select "Attach Shell"
#     exit<enter> or ctrl-c to exit from container

 Executing task: docker logs --tail 1000 -f c3d5e3f91cf4f0f38772647a41230ccf1d2bf000a5f2a45a87847586e05ea725 

'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
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
 * Debugger PIN: 124-475-803
192.168.195.11 - - [18/Mar/2023 19:17:53] "GET / HTTP/1.1" 404 -
192.168.195.11 - - [18/Mar/2023 19:19:29] "GET /api/activities/home HTTP/1.1" 200 -

#     ACCESS USING THE COMMAND LINE FAILED (TRY AGAIN LATER)

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ echo $CONTAINER_ID
c3d5e3f91cf4f0f38772647a41230ccf1d2bf000a5f2a45a87847586e05ea725
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker ps
CONTAINER ID   IMAGE           COMMAND                  CREATED          STATUS          PORTS                                       NAMES
c3d5e3f91cf4   backend-flask   "python3 -m flask ru…"   11 minutes ago   Up 11 minutes   0.0.0.0:4567->4567/tcp, :::4567->4567/tcp   youthful_sammet
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker exec $CONTAINER_ID -it /bin/bash
OCI runtime exec failed: exec failed: unable to start container process: exec: "-it": executable file not found in $PATH: unknown
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 


# INSTALLING NPM

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ cd frontend*
gitpod /workspace/aws-bootcamp-cruddur-2023/frontend-react-js (main) $ ls -l 
total 1504
-rw-r--r-- 1 gitpod gitpod     923 Mar 18 18:08 package.json
-rw-r--r-- 1 gitpod gitpod 1524661 Mar 18 18:08 package-lock.json
drwxr-xr-x 2 gitpod gitpod    4096 Mar 18 18:08 public
-rw-r--r-- 1 gitpod gitpod      32 Mar 18 18:08 README.md
drwxr-xr-x 4 gitpod gitpod     181 Mar 18 18:08 src
gitpod /workspace/aws-bootcamp-cruddur-2023/frontend-react-js (main) $ cat README.md
## Frontend React JS

gitpod /workspace/aws-bootcamp-cruddur-2023/frontend-react-js (main) $ cat README.md^C
gitpod /workspace/aws-bootcamp-cruddur-2023/frontend-react-js (main) $ 
gitpod /workspace/aws-bootcamp-cruddur-2023/frontend-react-js (main) $ 
gitpod /workspace/aws-bootcamp-cruddur-2023/frontend-react-js (main) $ 
gitpod /workspace/aws-bootcamp-cruddur-2023/frontend-react-js (main) $ 
gitpod /workspace/aws-bootcamp-cruddur-2023/frontend-react-js (main) $ 
gitpod /workspace/aws-bootcamp-cruddur-2023/frontend-react-js (main) $ npm i
npm WARN deprecated w3c-hr-time@1.0.2: Use your platform's native performance.now() and performance.timeOrigin.
npm WARN deprecated urix@0.1.0: Please see https://github.com/lydell/urix#deprecated
npm WARN deprecated topo@2.0.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm WARN deprecated uuid@3.4.0: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm WARN deprecated stable@0.1.8: Modern JS already guarantees Array#sort() is a stable sort, so this library is deprecated. See the compatibility table on MDN: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort#browser_compatibility
npm WARN deprecated source-map-url@0.4.1: See https://github.com/lydell/source-map-url#deprecated
npm WARN deprecated source-map-resolve@0.5.3: See https://github.com/lydell/source-map-resolve#deprecated
npm WARN deprecated resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
npm WARN deprecated sane@2.5.2: some dependency vulnerabilities fixed, support for node < 10 dropped, and newer ECMAScript syntax/features added
npm WARN deprecated request-promise-native@1.0.9: request-promise-native has been deprecated because it extends the now deprecated request package, see https://github.com/request/request/issues/3142
npm WARN deprecated querystring@0.2.0: The querystring API is considered Legacy. new code should use the URLSearchParams API instead.
npm WARN deprecated request@2.88.2: request has been deprecated, see https://github.com/request/request/issues/3142
npm WARN deprecated left-pad@1.3.0: use String.prototype.padStart()
npm WARN deprecated kleur@2.0.2: Please upgrade to kleur@3 or migrate to 'ansi-colors' if you prefer the old syntax. Visit <https://github.com/lukeed/kleur/releases/tag/v3.0.0\> for migration path(s).
npm WARN deprecated uglify-es@3.3.9: support for ECMAScript is superseded by `uglify-js` as of v3.13.0
npm WARN deprecated hoek@4.2.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm WARN deprecated har-validator@5.1.5: this library is no longer supported
npm WARN deprecated flatten@1.0.3: flatten is deprecated in favor of utility frameworks such as lodash.
npm WARN deprecated html-webpack-plugin@4.0.0-alpha.2: please switch to a stable version
npm WARN deprecated eslint-loader@2.1.1: This loader has been deprecated. Please use eslint-webpack-plugin
npm WARN deprecated circular-json@0.3.3: CircularJSON is in maintenance only, flatted is its successor.
npm WARN deprecated chokidar@2.1.8: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm WARN deprecated joi@11.4.0: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm WARN deprecated svgo@1.3.2: This SVGO version is no longer supported. Upgrade to v2.x.x.
npm WARN deprecated acorn-dynamic-import@3.0.0: This is probably built in to whatever tool you're using. If you still need it... idk
npm WARN deprecated babel-eslint@9.0.0: babel-eslint is now @babel/eslint-parser. This package will no longer receive updates.
npm WARN deprecated core-js@2.6.12: core-js@<3.23.3 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Some versions have web compatibility issues. Please, upgrade your dependencies to the actual version of core-js.
npm WARN deprecated core-js@2.6.4: core-js@<3.23.3 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Some versions have web compatibility issues. Please, upgrade your dependencies to the actual version of core-js.

added 1926 packages, and audited 1927 packages in 34s

103 packages are looking for funding
  run `npm fund` for details

78 vulnerabilities (13 low, 19 moderate, 42 high, 4 critical)

To address issues that do not require attention, run:
  npm audit fix

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.
npm notice 
npm notice New major version of npm available! 8.19.3 -> 9.6.2
npm notice Changelog: https://github.com/npm/cli/releases/tag/v9.6.2
npm notice Run npm install -g npm@9.6.2 to update!
npm notice 
gitpod /workspace/aws-bootcamp-cruddur-2023/frontend-react-js (main) $ 


# CREATED DOCKERFILE AT FRONTEND_REACT.JS/DOCKERFILE
# --------------------------------------------------

FROM node:16.18

ENV PORT=3000

COPY . /frontend-react-js
WORKDIR /frontend-react-js
RUN npm install
EXPOSE ${PORT}
CMD ["npm", "start"]

# BUILD FRONTEND_REACT.js

gitpod /workspace/aws-bootcamp-cruddur-2023/frontend-react-js (main) $ docker build -t frontend-react-js ./frontend-react-js
unable to prepare context: path "./frontend-react-js" not found
gitpod /workspace/aws-bootcamp-cruddur-2023/frontend-react-js (main) $ cd ..
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker build -t frontend-react-js ./frontend-react-js
Sending build context to Docker daemon  236.1MB
Step 1/7 : FROM node:16.18
16.18: Pulling from library/node
620af4e91dbf: Pull complete 
fae29f309a72: Pull complete 
28fca74d99b6: Pull complete 
0b5db87f5b42: Pull complete 
fa488706ea13: Pull complete 
0380b9b3282f: Pull complete 
383dfecd3687: Pull complete 
ca59981dc274: Pull complete 
4fa5c4b55a85: Pull complete 
Digest: sha256:7f404d09ceb780c51f4fac7592c46b8f21211474aacce25389eb0df06aaa7472
Status: Downloaded newer image for node:16.18
 ---> 993a4cf9c1e8
Step 2/7 : ENV PORT=3000
 ---> Running in a8e33c2b03a0
Removing intermediate container a8e33c2b03a0
 ---> b9274123cd2a
Step 3/7 : COPY . /frontend-react-js
 ---> 8a6e1c9eed6b
Step 4/7 : WORKDIR /frontend-react-js
 ---> Running in c9751ddb2045
Removing intermediate container c9751ddb2045
 ---> 30b3144457ad
Step 5/7 : RUN npm install
 ---> Running in 3f0b00545b37

up to date, audited 1927 packages in 7s

103 packages are looking for funding
  run `npm fund` for details

78 vulnerabilities (13 low, 19 moderate, 42 high, 4 critical)

To address issues that do not require attention, run:
  npm audit fix

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.
npm notice 
npm notice New major version of npm available! 8.19.2 -> 9.6.2
npm notice Changelog: <https://github.com/npm/cli/releases/tag/v9.6.2>
npm notice Run `npm install -g npm@9.6.2` to update!
npm notice 
Removing intermediate container 3f0b00545b37
 ---> 0a53f4e8420d
Step 6/7 : EXPOSE ${PORT}
 ---> Running in 5789c9c35e22
Removing intermediate container 5789c9c35e22
 ---> c3b74a4c150e
Step 7/7 : CMD ["npm", "start"]
 ---> Running in d80d801844a6
Removing intermediate container d80d801844a6
 ---> ccce78c61614
Successfully built ccce78c61614
Successfully tagged frontend-react-js:latest
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 

# RUN FRONTEND_REACT.js

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker run -p 3000:3000 -d frontend-react-js^C
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docket images
bash: docket: command not found
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker images
REPOSITORY          TAG                IMAGE ID       CREATED              SIZE
frontend-react-js   latest             ccce78c61614   About a minute ago   1.14GB
backend-flask       latest             4938dada5ebc   About an hour ago    130MB
python              3.10-slim-buster   83773ada8884   41 hours ago         118MB
node                16.18              993a4cf9c1e8   3 months ago         910MB
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker ps
CONTAINER ID   IMAGE           COMMAND                  CREATED          STATUS          PORTS                                       NAMES
c3d5e3f91cf4   backend-flask   "python3 -m flask ru…"   27 minutes ago   Up 27 minutes   0.0.0.0:4567->4567/tcp, :::4567->4567/tcp   youthful_sammet
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker run -p 3000:3000 -d frontend-react-js
b1f6268f1ccbc270086bbcc84eccb07ca64a33ed7149b81a67ca01337ef7d0a8
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 

# DOCKER LOG FOR FRONTEND_REACT CONTAINER EXECUTION

 *  Executing task: docker logs --tail 1000 -f f4f539aea4af448df3e99b831a1c5190e9c097d60a39eaf02f5a7f018f401a0b 


> frontend@0.1.0 start
> react-scripts start

(node:44) [DEP0111] DeprecationWarning: Access to process.binding('http_parser') is deprecated.
(Use `node --trace-deprecation ...` to show where the warning was created)
Starting the development server...

Failed to compile.

./src/components/ActivityActionRepost.js
  Line 10:  'React' must be in scope when using JSX  react/react-in-jsx-scope
  Line 14:   'React' must be in scope when using JSX  react/react-in-jsx-scope
  Line 15:   'React' must be in scope when using JSX  react/react-in-jsx-scope

Search for the keywords to learn more about each error.

# frontend-react/package.json
#   Errors during frontend container execution were caused by modification of react-scripts version
#   to ^2.1.3 from the original value of 5.0.1 (possibly caused by execution of "npm install" when
#   creating node_modules).  react-scripts version reverted to "5.0.1" (as in omenking's original
#   version).

{
  "name": "frontend",
  "version": "0.1.0",
  "private": true,
  "dependencies": {
    "@testing-library/jest-dom": "^5.16.5",
    "@testing-library/react": "^13.4.0",
    "@testing-library/user-event": "^13.5.0",
    "js-cookie": "^3.0.1",
    "luxon": "^3.1.0",
    "process": "^0.11.10",
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "react-router-dom": "^6.4.3",
    "react-scripts": "5.0.1",
    "web-vitals": "^2.1.4"
  },
  "scripts": {
    "start": "react-scripts start",
    "build": "react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject"
  },
  "eslintConfig": {
    "extends": [
      "react-app",
      "react-app/jest"
    ]
  },
  "browserslist": {
    "production": [
      ">0.2%",
      "not dead",
      "not op_mini all"
    ],
    "development": [
      "last 1 chrome version",
      "last 1 firefox version",
      "last 1 safari version"
    ]
  }
}

# NEW RUN OF [NPM INSTALL] AFTER FIX
# ----------------------------------

gitpod /workspace/aws-bootcamp-cruddur-2023/frontend-react-js (main) $ npm i
npm WARN deprecated rollup-plugin-terser@7.0.2: This package has been deprecated and is no longer maintained. Please use @rollup/plugin-terser
npm WARN deprecated sourcemap-codec@1.4.8: Please use @jridgewell/sourcemap-codec instead

added 576 packages, removed 1014 packages, changed 351 packages, and audited 1489 packages in 29s

230 packages are looking for funding
  run `npm fund` for details

6 high severity vulnerabilities

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.
npm notice 
npm notice New major version of npm available! 8.19.3 -> 9.6.2
npm notice Changelog: https://github.com/npm/cli/releases/tag/v9.6.2
npm notice Run npm install -g npm@9.6.2 to update!
npm notice 
gitpod /workspace/aws-bootcamp-cruddur-2023/frontend-react-js (main) $ 


# BUILD FRONTEND-REACT 

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker build -t frontend-react-js ./frontend-react-js
Sending build context to Docker daemon  242.1MB
Step 1/7 : FROM node:16.18
 ---> 993a4cf9c1e8
Step 2/7 : ENV PORT=3000
 ---> Using cache
 ---> b9274123cd2a
Step 3/7 : COPY . /frontend-react-js
 ---> 7ad4d1e95eea
Step 4/7 : WORKDIR /frontend-react-js
 ---> Running in 47bceaf57435
Removing intermediate container 47bceaf57435
 ---> 2846c3d7a9b6
Step 5/7 : RUN npm install
 ---> Running in 988b5f32168a

changed 1 package, and audited 1489 packages in 5s

230 packages are looking for funding
  run `npm fund` for details

6 high severity vulnerabilities

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.
npm notice 
npm notice New major version of npm available! 8.19.2 -> 9.6.2
npm notice Changelog: <https://github.com/npm/cli/releases/tag/v9.6.2>
npm notice Run `npm install -g npm@9.6.2` to update!
npm notice 
Removing intermediate container 988b5f32168a
 ---> 55ee406f3a38
Step 6/7 : EXPOSE ${PORT}
 ---> Running in fc03ed0f5edb
Removing intermediate container fc03ed0f5edb
 ---> ab3b96b54b5b
Step 7/7 : CMD ["npm", "start"]
 ---> Running in 059dd841e40e
Removing intermediate container 059dd841e40e
 ---> 04f9c7671cf1
Successfully built 04f9c7671cf1
Successfully tagged frontend-react-js:latest
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker images
REPOSITORY          TAG                IMAGE ID       CREATED         SIZE
frontend-react-js   latest             04f9c7671cf1   2 minutes ago   1.21GB
<none>              <none>             ccce78c61614   32 hours ago    1.14GB
backend-flask       latest             4938dada5ebc   34 hours ago    130MB
python              3.10-slim-buster   83773ada8884   3 days ago      118MB
node                16.18              993a4cf9c1e8   3 months ago    910MB
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker ps
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS    NAMES
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker ps -a
CONTAINER ID   IMAGE          COMMAND                  CREATED        STATUS                    PORTS     NAMES
f4f539aea4af   ccce78c61614   "docker-entrypoint.s…"   32 hours ago   Exited (1) 32 hours ago             mystifying_booth
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ docker compose up
[+] Building 29.4s (18/18) FINISHED                                                                                                                                  
 => [aws-bootcamp-cruddur-2023-backend-flask internal] load build definition from Dockerfile                                                                    0.0s
 => => transferring dockerfile: 294B                                                                                                                            0.0s
 => [aws-bootcamp-cruddur-2023-frontend-react-js internal] load build definition from Dockerfile                                                                0.0s
 => => transferring dockerfile: 176B                                                                                                                            0.0s
 => [aws-bootcamp-cruddur-2023-backend-flask internal] load .dockerignore                                                                                       0.0s
 => => transferring context: 2B                                                                                                                                 0.0s
 => [aws-bootcamp-cruddur-2023-frontend-react-js internal] load .dockerignore                                                                                   0.0s
 => => transferring context: 2B                                                                                                                                 0.0s
 => [aws-bootcamp-cruddur-2023-backend-flask internal] load metadata for docker.io/library/python:3.10-slim-buster                                              0.0s
 => [aws-bootcamp-cruddur-2023-backend-flask 1/5] FROM docker.io/library/python:3.10-slim-buster                                                                0.2s
 => [aws-bootcamp-cruddur-2023-backend-flask internal] load build context                                                                                       0.0s
 => => transferring context: 19.78kB                                                                                                                            0.0s
 => [aws-bootcamp-cruddur-2023-frontend-react-js internal] load metadata for docker.io/library/node:16.18                                                       0.0s
 => [aws-bootcamp-cruddur-2023-frontend-react-js internal] load build context                                                                                  11.4s
 => => transferring context: 213.47MB                                                                                                                          11.3s
 => [aws-bootcamp-cruddur-2023-frontend-react-js 1/4] FROM docker.io/library/node:16.18                                                                         0.5s
 => [aws-bootcamp-cruddur-2023-backend-flask 2/5] WORKDIR /backend-flask                                                                                        0.2s
 => [aws-bootcamp-cruddur-2023-backend-flask 3/5] COPY requirements.txt requirements.txt                                                                        0.2s
 => [aws-bootcamp-cruddur-2023-backend-flask 4/5] RUN pip3 install -r requirements.txt                                                                         10.5s
 => [aws-bootcamp-cruddur-2023-backend-flask 5/5] COPY . .                                                                                                      0.2s 
 => [aws-bootcamp-cruddur-2023-frontend-react-js] exporting to image                                                                                            8.5s
 => => exporting layers                                                                                                                                         7.5s
 => => writing image sha256:1df98b1ca46e5bcac71d1b97f434f52403663e331a3c8d1b5264969fad9c9799                                                                    0.0s
 => => naming to docker.io/library/aws-bootcamp-cruddur-2023-backend-flask                                                                                      0.0s
 => => writing image sha256:c267236c1ef2936db045ba0238573841fdee0a47caec33ef66281db612665ef9                                                                    0.0s
 => => naming to docker.io/library/aws-bootcamp-cruddur-2023-frontend-react-js                                                                                  0.0s
 => [aws-bootcamp-cruddur-2023-frontend-react-js 2/4] COPY . /frontend-react-js                                                                                 4.4s
 => [aws-bootcamp-cruddur-2023-frontend-react-js 3/4] WORKDIR /frontend-react-js                                                                                0.1s
 => [aws-bootcamp-cruddur-2023-frontend-react-js 4/4] RUN npm install                                                                                           5.7s
[+] Running 3/1
 ✔ Network aws-bootcamp-cruddur-2023_default                Created                                                                                             0.0s 
 ✔ Container aws-bootcamp-cruddur-2023-backend-flask-1      Created                                                                                             0.0s 
 ✔ Container aws-bootcamp-cruddur-2023-frontend-react-js-1  Created                                                                                             0.0s 
Attaching to aws-bootcamp-cruddur-2023-backend-flask-1, aws-bootcamp-cruddur-2023-frontend-react-js-1
aws-bootcamp-cruddur-2023-backend-flask-1      | 'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
aws-bootcamp-cruddur-2023-backend-flask-1      | 'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
aws-bootcamp-cruddur-2023-backend-flask-1      | 'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
aws-bootcamp-cruddur-2023-backend-flask-1      |  * Debug mode: on
aws-bootcamp-cruddur-2023-backend-flask-1      | WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
aws-bootcamp-cruddur-2023-backend-flask-1      |  * Running on all addresses (0.0.0.0)
aws-bootcamp-cruddur-2023-backend-flask-1      |  * Running on http://127.0.0.1:4567
aws-bootcamp-cruddur-2023-backend-flask-1      |  * Running on http://172.18.0.3:4567
aws-bootcamp-cruddur-2023-backend-flask-1      | Press CTRL+C to quit
aws-bootcamp-cruddur-2023-backend-flask-1      |  * Restarting with stat
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | > frontend@0.1.0 start
aws-bootcamp-cruddur-2023-frontend-react-js-1  | > react-scripts start
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-backend-flask-1      | 'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
aws-bootcamp-cruddur-2023-backend-flask-1      | 'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
aws-bootcamp-cruddur-2023-backend-flask-1      | 'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
aws-bootcamp-cruddur-2023-backend-flask-1      |  * Debugger is active!
aws-bootcamp-cruddur-2023-backend-flask-1      |  * Debugger PIN: 900-683-431
aws-bootcamp-cruddur-2023-frontend-react-js-1  | (node:44) [DEP_WEBPACK_DEV_SERVER_ON_AFTER_SETUP_MIDDLEWARE] DeprecationWarning: 'onAfterSetupMiddleware' option is deprecated. Please use the 'setupMiddlewares' option.
aws-bootcamp-cruddur-2023-frontend-react-js-1  | (Use `node --trace-deprecation ...` to show where the warning was created)
aws-bootcamp-cruddur-2023-frontend-react-js-1  | (node:44) [DEP_WEBPACK_DEV_SERVER_ON_BEFORE_SETUP_MIDDLEWARE] DeprecationWarning: 'onBeforeSetupMiddleware' option is deprecated. Please use the 'setupMiddlewares' option.
aws-bootcamp-cruddur-2023-frontend-react-js-1  | Starting the development server...
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | Compiled with warnings.
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | Warning
aws-bootcamp-cruddur-2023-frontend-react-js-1  | (4:3) autoprefixer: start value has mixed support, consider using flex-start instead
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | Warning
aws-bootcamp-cruddur-2023-frontend-react-js-1  | (3:3) autoprefixer: start value has mixed support, consider using flex-start instead
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | Warning
aws-bootcamp-cruddur-2023-frontend-react-js-1  | (3:3) autoprefixer: start value has mixed support, consider using flex-start instead
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | [eslint] 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/App.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 12:8:  'process' is defined but never used  no-unused-vars
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/components/DesktopNavigationLink.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 18:5:  Expected a default case  default-case
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 21:9:  Unreachable code         no-unreachable
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 24:9:  Unreachable code         no-unreachable
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 27:9:  Unreachable code         no-unreachable
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 30:9:  Unreachable code         no-unreachable
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 33:9:  Unreachable code         no-unreachable
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/components/DesktopSidebar.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 41:9:  The href attribute requires a valid value to be accessible. Provide a valid, navigable address as the href value. If you cannot provide a valid href, but still need the element to resemble a link, use a button and change it with appropriate styles. Learn more: https://github.com/jsx-eslint/eslint-plugin-jsx-a11y/blob/HEAD/docs/rules/anchor-is-valid.md  jsx-a11y/anchor-is-valid
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 42:9:  The href attribute requires a valid value to be accessible. Provide a valid, navigable address as the href value. If you cannot provide a valid href, but still need the element to resemble a link, use a button and change it with appropriate styles. Learn more: https://github.com/jsx-eslint/eslint-plugin-jsx-a11y/blob/HEAD/docs/rules/anchor-is-valid.md  jsx-a11y/anchor-is-valid
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 43:9:  The href attribute requires a valid value to be accessible. Provide a valid, navigable address as the href value. If you cannot provide a valid href, but still need the element to resemble a link, use a button and change it with appropriate styles. Learn more: https://github.com/jsx-eslint/eslint-plugin-jsx-a11y/blob/HEAD/docs/rules/anchor-is-valid.md  jsx-a11y/anchor-is-valid
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/components/MessageGroupItem.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 27:23:  Expected '===' and instead saw '=='  eqeqeq
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/components/ProfileInfo.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 29:16:  Expected '===' and instead saw '=='  eqeqeq
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/components/ReplyForm.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 4:27:  'BombIcon' is defined but never used  no-unused-vars
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/components/TrendItem.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 13:5:  The href attribute requires a valid value to be accessible. Provide a valid, navigable address as the href value. If you cannot provide a valid href, but still need the element to resemble a link, use a button and change it with appropriate styles. Learn more: https://github.com/jsx-eslint/eslint-plugin-jsx-a11y/blob/HEAD/docs/rules/anchor-is-valid.md  jsx-a11y/anchor-is-valid
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/pages/ConfirmationPage.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 13:20:  'setCodeSent' is assigned a value but never used                                                                       no-unused-vars
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 67:6:   React Hook React.useEffect has a missing dependency: 'params.email'. Either include it or remove the dependency array  react-hooks/exhaustive-deps
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/pages/MessageGroupPage.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 16:10:  'popped' is assigned a value but never used                                                                                    no-unused-vars
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 75:6:   React Hook React.useEffect has a missing dependency: 'loadMessageGroupData'. Either include it or remove the dependency array  react-hooks/exhaustive-deps
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/pages/MessageGroupsPage.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 12:10:  'popped' is assigned a value but never used  no-unused-vars
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/pages/RecoverPage.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 12:18:   'setErrors' is assigned a value but never used     no-unused-vars
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 13:21:   'setFormState' is assigned a value but never used  no-unused-vars
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 118:17:  Expected '===' and instead saw '=='                eqeqeq
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 121:22:  Expected '===' and instead saw '=='                eqeqeq
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 124:22:  Expected '===' and instead saw '=='                eqeqeq
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/pages/SignupPage.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 16:18:  'setErrors' is assigned a value but never used  no-unused-vars
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/pages/UserFeedPage.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 57:6:  React Hook React.useEffect has a missing dependency: 'loadData'. Either include it or remove the dependency array  react-hooks/exhaustive-deps
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | Search for the keywords to learn more about each warning.
aws-bootcamp-cruddur-2023-frontend-react-js-1  | To ignore, add // eslint-disable-next-line to the line before.
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | WARNING in ./src/components/ActivityContent.css (./node_modules/css-loader/dist/cjs.js??ruleSet[1].rules[1].oneOf[5].use[1]!./node_modules/postcss-loader/dist/cjs.js??ruleSet[1].rules[1].oneOf[5].use[2]!./node_modules/source-map-loader/dist/cjs.js!./src/components/ActivityContent.css)
aws-bootcamp-cruddur-2023-frontend-react-js-1  | Module Warning (from ./node_modules/postcss-loader/dist/cjs.js):
aws-bootcamp-cruddur-2023-frontend-react-js-1  | Warning
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | (4:3) autoprefixer: start value has mixed support, consider using flex-start instead
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | WARNING in ./src/components/MessageGroupItem.css (./node_modules/css-loader/dist/cjs.js??ruleSet[1].rules[1].oneOf[5].use[1]!./node_modules/postcss-loader/dist/cjs.js??ruleSet[1].rules[1].oneOf[5].use[2]!./node_modules/source-map-loader/dist/cjs.js!./src/components/MessageGroupItem.css)
aws-bootcamp-cruddur-2023-frontend-react-js-1  | Module Warning (from ./node_modules/postcss-loader/dist/cjs.js):
aws-bootcamp-cruddur-2023-frontend-react-js-1  | Warning
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | (3:3) autoprefixer: start value has mixed support, consider using flex-start instead
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | WARNING in ./src/components/MessageItem.css (./node_modules/css-loader/dist/cjs.js??ruleSet[1].rules[1].oneOf[5].use[1]!./node_modules/postcss-loader/dist/cjs.js??ruleSet[1].rules[1].oneOf[5].use[2]!./node_modules/source-map-loader/dist/cjs.js!./src/components/MessageItem.css)
aws-bootcamp-cruddur-2023-frontend-react-js-1  | Module Warning (from ./node_modules/postcss-loader/dist/cjs.js):
aws-bootcamp-cruddur-2023-frontend-react-js-1  | Warning
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | (3:3) autoprefixer: start value has mixed support, consider using flex-start instead
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | WARNING in [eslint] 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/App.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 12:8:  'process' is defined but never used  no-unused-vars
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/components/DesktopNavigationLink.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 18:5:  Expected a default case  default-case
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 21:9:  Unreachable code         no-unreachable
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 24:9:  Unreachable code         no-unreachable
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 27:9:  Unreachable code         no-unreachable
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 30:9:  Unreachable code         no-unreachable
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 33:9:  Unreachable code         no-unreachable
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/components/DesktopSidebar.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 41:9:  The href attribute requires a valid value to be accessible. Provide a valid, navigable address as the href value. If you cannot provide a valid href, but still need the element to resemble a link, use a button and change it with appropriate styles. Learn more: https://github.com/jsx-eslint/eslint-plugin-jsx-a11y/blob/HEAD/docs/rules/anchor-is-valid.md  jsx-a11y/anchor-is-valid
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 42:9:  The href attribute requires a valid value to be accessible. Provide a valid, navigable address as the href value. If you cannot provide a valid href, but still need the element to resemble a link, use a button and change it with appropriate styles. Learn more: https://github.com/jsx-eslint/eslint-plugin-jsx-a11y/blob/HEAD/docs/rules/anchor-is-valid.md  jsx-a11y/anchor-is-valid
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 43:9:  The href attribute requires a valid value to be accessible. Provide a valid, navigable address as the href value. If you cannot provide a valid href, but still need the element to resemble a link, use a button and change it with appropriate styles. Learn more: https://github.com/jsx-eslint/eslint-plugin-jsx-a11y/blob/HEAD/docs/rules/anchor-is-valid.md  jsx-a11y/anchor-is-valid
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/components/MessageGroupItem.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 27:23:  Expected '===' and instead saw '=='  eqeqeq
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/components/ProfileInfo.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 29:16:  Expected '===' and instead saw '=='  eqeqeq
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/components/ReplyForm.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 4:27:  'BombIcon' is defined but never used  no-unused-vars
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/components/TrendItem.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 13:5:  The href attribute requires a valid value to be accessible. Provide a valid, navigable address as the href value. If you cannot provide a valid href, but still need the element to resemble a link, use a button and change it with appropriate styles. Learn more: https://github.com/jsx-eslint/eslint-plugin-jsx-a11y/blob/HEAD/docs/rules/anchor-is-valid.md  jsx-a11y/anchor-is-valid
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/pages/ConfirmationPage.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 13:20:  'setCodeSent' is assigned a value but never used                                                                       no-unused-vars
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 67:6:   React Hook React.useEffect has a missing dependency: 'params.email'. Either include it or remove the dependency array  react-hooks/exhaustive-deps
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/pages/MessageGroupPage.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 16:10:  'popped' is assigned a value but never used                                                                                    no-unused-vars
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 75:6:   React Hook React.useEffect has a missing dependency: 'loadMessageGroupData'. Either include it or remove the dependency array  react-hooks/exhaustive-deps
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/pages/MessageGroupsPage.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 12:10:  'popped' is assigned a value but never used  no-unused-vars
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/pages/RecoverPage.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 12:18:   'setErrors' is assigned a value but never used     no-unused-vars
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 13:21:   'setFormState' is assigned a value but never used  no-unused-vars
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 118:17:  Expected '===' and instead saw '=='                eqeqeq
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 121:22:  Expected '===' and instead saw '=='                eqeqeq
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 124:22:  Expected '===' and instead saw '=='                eqeqeq
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/pages/SignupPage.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 16:18:  'setErrors' is assigned a value but never used  no-unused-vars
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | src/pages/UserFeedPage.js
aws-bootcamp-cruddur-2023-frontend-react-js-1  |   Line 57:6:  React Hook React.useEffect has a missing dependency: 'loadData'. Either include it or remove the dependency array  react-hooks/exhaustive-deps
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | webpack compiled with 4 warnings
aws-bootcamp-cruddur-2023-backend-flask-1      | 192.168.105.142 - - [20/Mar/2023 04:13:28] "GET / HTTP/1.1" 404 -
aws-bootcamp-cruddur-2023-backend-flask-1      | 192.168.105.142 - - [20/Mar/2023 04:13:57] "GET /api/activities/home HTTP/1.1" 200 -
aws-bootcamp-cruddur-2023-backend-flask-1      | 192.168.105.142 - - [20/Mar/2023 04:14:20] "GET /api/activities/home HTTP/1.1" 200 -
^CGracefully stopping... (press Ctrl+C again to force)
Aborting on container exit...
[+] Running 2/2
 ✔ Container aws-bootcamp-cruddur-2023-backend-flask-1      Stopped                                                                                             0.3s 
 ✔ Container aws-bootcamp-cruddur-2023-frontend-react-js-1  Stopped                                                                                             0.8s 
canceled
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 

# ==========================================
# DYNAMODB DOCUMENTATION FROM 100DaysOfCloud
# ==========================================

Run Docker Local

docker-compose up

Create a table

aws dynamodb create-table \
    --endpoint-url http://localhost:8000 \
    --table-name Music \
    --attribute-definitions \
        AttributeName=Artist,AttributeType=S \
        AttributeName=SongTitle,AttributeType=S \
    --key-schema AttributeName=Artist,KeyType=HASH AttributeName=SongTitle,KeyType=RANGE \
    --provisioned-throughput ReadCapacityUnits=1,WriteCapacityUnits=1 \
    --table-class STANDARD

Create an Item

aws dynamodb put-item \
    --endpoint-url http://localhost:8000 \
    --table-name Music \
    --item \
        '{"Artist": {"S": "No One You Know"}, "SongTitle": {"S": "Call Me Today"}, "AlbumTitle": {"S": "Somewhat Famous"}}' \
    --return-consumed-capacity TOTAL  

List Tables

aws dynamodb list-tables --endpoint-url http://localhost:8000

Get Records

aws dynamodb scan --table-name cruddur_cruds --query "Items" --endpoint-url http://localhost:8000

References

https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.html https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Tools.CLI.html

NOTE: Table name was screwed up.  List table command shows "cruddur cruds" for the name but it is actually named "Music".

# =============================
# POSTGRESS CLIENT INSTALLATION
# =============================

- name: postgres
    init: |
      curl -fsSL https://www.postgresql.org/media/keys/ACCC4CF8.asc|sudo gpg --dearmor -o /etc/apt/trusted.gpg.d/postgresql.gpg
      echo "deb http://apt.postgresql.org/pub/repos/apt/ `lsb_release -cs`-pgdg main" |sudo tee  /etc/apt/sources.list.d/pgdg.list
      sudo apt update
      sudo apt install -y postgresql-client-13 libpq-dev

# ==========================================================
# DYNAMODB AND POSTGRESS INTEGRATED INTO DOCKER COMPOSE FILE
# ==========================================================

version: "3.8"
# ------------------------------------------------
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
  dynamodb-local:
    # https://stackoverflow.com/questions/67533058/persist-local-dynamodb-data-in-volumes-lack-permission-unable-to-open-databa
    # We needed to add user:root to get this working.
    user: root
    command: "-jar DynamoDBLocal.jar -sharedDb -dbPath ./data"
    image: "amazon/dynamodb-local:latest"
    container_name: dynamodb-local
    ports:
      - "8000:8000"
    volumes:
      - "./docker/dynamodb:/home/dynamodblocal/data"
    working_dir: /home/dynamodblocal
  db:
    image: postgres:13-alpine
    restart: always
    environment:
      - POSTGRES_USER=postgres
      - POSTGRES_PASSWORD=password
    ports:
      - '5432:5432'
    volumes: 
      - db:/var/lib/postgresql/data
# ------------------------------------------------
volumes:
  db:
    driver: local
# ------------------------------------------------
# the name flag is a hack to change the default prepend folder
# name when outputting the image names
networks: 
  internal-network:
    driver: bridge
    name: cruddur

# ==========================================================
# POSTGRESS CLIENT STARTUP INTEGRATED INTO GITPOD.YML
# ==========================================================

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
  - name: postgres
    init: |
      curl -fsSL https://www.postgresql.org/media/keys/ACCC4CF8.asc|sudo gpg --dearmor -o /etc/apt/trusted.gpg.d/postgresql.gpg
      echo "deb http://apt.postgresql.org/pub/repos/apt/ `lsb_release -cs`-pgdg main" |sudo tee  /etc/apt/sources.list.d/pgdg.list
      sudo apt update
      sudo apt install -y postgresql-client-13 libpq-dev
vscode:
  extensions:
    - 42Crunch.vscode-openapi
    - ms-azuretools.vscode-docker

# END OF FILE

      