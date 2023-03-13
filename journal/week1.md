# Week 1 — App Containerization


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


https://4567-burreetoman-awsbootcamp-4p5m4koar62.ws-us90.gitpod.io/api/activities/home

[{"created_at":"2023-03-11T04:36:22.382080+00:00","expires_at":"2023-03-18T04:36:22.382080+00:00","handle":"Andrew Brown","likes_count":5,"message":"Cloud is fun!","replies":[{"created_at":"2023-03-11T04:36:22.382080+00:00","handle":"Worf","likes_count":0,"message":"This post has no honor!","replies_count":0,"reply_to_activity_uuid":"68f126b0-1ceb-4a33-88be-d90fa7109eee","reposts_count":0,"uuid":"26e12864-1c26-5c3a-9658-97a10f8fea67"}],"replies_count":1,"reposts_count":0,"uuid":"68f126b0-1ceb-4a33-88be-d90fa7109eee"},{"created_at":"2023-03-06T04:36:22.382080+00:00","expires_at":"2023-03-22T04:36:22.382080+00:00","handle":"Worf","likes":0,"message":"I am out of prune juice","replies":[],"uuid":"66e12864-8c26-4c3a-9658-95a10f8fea67"},{"created_at":"2023-03-13T03:36:22.382080+00:00","expires_at":"2023-03-13T16:36:22.382080+00:00","handle":"Garek","likes":0,"message":"My dear doctor, I am just simple tailor","replies":[],"uuid":"248959df-3079-4947-b847-9e0892d1bab4"}]


unset FRONTEND_URL
unset BACKEND_URL


