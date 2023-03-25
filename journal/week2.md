# Week 2 — Distributed Tracing


gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ export HONEYCOMB_API_KEY="ovnK5dcmiodHM75hiEFFmC"
gitpod /workspace/aws-bootcamp-cruddur-2023 (mgp env MB_API_KEY="ovnK5dcmiodHM75hiEFFmC"
bash: egp: command not found
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ gp env HONEYCOMB_API_KEY="ovnK5dcmiodHM75hiEFFmC"
HONEYCOMB_API_KEY=ovnK5dcmiodHM75hiEFFmC
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ env
PYENV_HOOK_PATH=/home/gitpod/.gp_pyenv.d
PIPENV_VENV_IN_PROJECT=true
GP_PREVIEW_BROWSER=/ide/bin/remote-cli/gitpod-code --preview
PYENV_SHELL=bash
rvm_prefix=/home/gitpod
SUPERVISOR_ADDR=localhost:22999
HOSTNAME=burreetoman-awsbootcamp-81p8i5r1rli
GITPOD_REPO_ROOT=/workspace/aws-bootcamp-cruddur-2023
JAVA_HOME=/home/gitpod/.sdkman/candidates/java/current
WORKSPACEKIT_WRAP_NETNS=true
GRADLE_HOME=/home/gitpod/.sdkman/candidates/gradle/current
GITPOD_ANALYTICS_WRITER=segment
TRIGGER_REBUILD=1
AWS_DEFAULT_REGION=us-west-2
GP_PYENV_FAKEROOT=/workspace/.pyenv_mirror/fakeroot
MY_RUBY_HOME=/home/gitpod/.rvm/rubies/ruby-3.1.2
THEIA_RATELIMIT_LOG=50
SDKMAN_CANDIDATES_DIR=/home/gitpod/.sdkman/candidates
HONEYCOMB_API_KEY=ovnK5dcmiodHM75hiEFFmC
GP_PYENV_INIT=true
NIX_VERSION=2.11.0
EDITOR=/ide/bin/remote-cli/gitpod-code
RUBY_VERSION=ruby-3.1.2
GITPOD_WORKSPACE_CLASS_INFO={"id":"g1-standard","category":"GENERAL PURPOSE","displayName":"Standard","description":"Up to 4 cores, 8GB RAM, 30GB storage","powerups":1,"isDefault":true,"deprecated":false}
PWD=/workspace/aws-bootcamp-cruddur-2023
NIX_PROFILES=/nix/var/nix/profiles/default /home/gitpod/.nix-profile
THEIA_WORKSPACE_ROOT=/workspace/aws-bootcamp-cruddur-2023
GITPOD_PREVENT_METADATA_ACCESS=true
GP_OPEN_EDITOR=/ide/bin/remote-cli/gitpod-code
rvm_version=1.29.12 (latest)
MANPATH=/home/gitpod/.nix-profile/share/man::/home/linuxbrew/.linuxbrew/share/man
PNPM_HOME=/home/gitpod/.pnpm
PYTHONUSERBASE_VERSION_FILE=/workspace/.pyenv_mirror/user/.mounted_version
GP_EXTERNAL_BROWSER=/ide/bin/remote-cli/gitpod-code --openExternal
GITPOD_OWNER_ID=73eeed64-1933-4d39-b9f7-c0e40048fbfd
HOME=/home/gitpod
LANG=en_US.UTF-8
GITPOD_WORKSPACE_ID=burreetoman-awsbootcamp-81p8i5r1rli
GITPOD_INTERVAL=30000
LS_COLORS=rs=0:di=01;34:ln=01;36:mh=00:pi=40;33:so=01;35:do=01;35:bd=40;33;01:cd=40;33;01:or=40;31;01:mi=00:su=37;41:sg=30;43:ca=30;41:tw=30;42:ow=34;42:st=37;44:ex=01;32:*.tar=01;31:*.tgz=01;31:*.arc=01;31:*.arj=01;31:*.taz=01;31:*.lha=01;31:*.lz4=01;31:*.lzh=01;31:*.lzma=01;31:*.tlz=01;31:*.txz=01;31:*.tzo=01;31:*.t7z=01;31:*.zip=01;31:*.z=01;31:*.dz=01;31:*.gz=01;31:*.lrz=01;31:*.lz=01;31:*.lzo=01;31:*.xz=01;31:*.zst=01;31:*.tzst=01;31:*.bz2=01;31:*.bz=01;31:*.tbz=01;31:*.tbz2=01;31:*.tz=01;31:*.deb=01;31:*.rpm=01;31:*.jar=01;31:*.war=01;31:*.ear=01;31:*.sar=01;31:*.rar=01;31:*.alz=01;31:*.ace=01;31:*.zoo=01;31:*.cpio=01;31:*.7z=01;31:*.rz=01;31:*.cab=01;31:*.wim=01;31:*.swm=01;31:*.dwm=01;31:*.esd=01;31:*.jpg=01;35:*.jpeg=01;35:*.mjpg=01;35:*.mjpeg=01;35:*.gif=01;35:*.bmp=01;35:*.pbm=01;35:*.pgm=01;35:*.ppm=01;35:*.tga=01;35:*.xbm=01;35:*.xpm=01;35:*.tif=01;35:*.tiff=01;35:*.png=01;35:*.svg=01;35:*.svgz=01;35:*.mng=01;35:*.pcx=01;35:*.mov=01;35:*.mpg=01;35:*.mpeg=01;35:*.m2v=01;35:*.mkv=01;35:*.webm=01;35:*.ogm=01;35:*.mp4=01;35:*.m4v=01;35:*.mp4v=01;35:*.vob=01;35:*.qt=01;35:*.nuv=01;35:*.wmv=01;35:*.asf=01;35:*.rm=01;35:*.rmvb=01;35:*.flc=01;35:*.avi=01;35:*.fli=01;35:*.flv=01;35:*.gl=01;35:*.dl=01;35:*.xcf=01;35:*.xwd=01;35:*.yuv=01;35:*.cgm=01;35:*.emf=01;35:*.ogv=01;35:*.ogx=01;35:*.aac=00;36:*.au=00;36:*.flac=00;36:*.m4a=00;36:*.mid=00;36:*.midi=00;36:*.mka=00;36:*.mp3=00;36:*.mpc=00;36:*.ogg=00;36:*.ra=00;36:*.wav=00;36:*.oga=00;36:*.opus=00;36:*.spx=00;36:*.xspf=00;36:
CARGO_HOME=/workspace/.cargo
GITPOD_WORKSPACE_CONTEXT_URL=https://github.com/burreetoman/aws-bootcamp-cruddur-2023
THEIA_MINI_BROWSER_HOST_PATTERN=browser-{{hostname}}
NIX_SSL_CERT_FILE=/etc/ssl/certs/ca-certificates.crt
SDKMAN_VERSION=5.16.0
GITPOD_WORKSPACE_CLASS=g1-standard
AWS_SECRET_ACCESS_KEY=2V9P9YnabHLUhGgjogtn8i6FJ8HKkIi+hC243H31
GITPOD_INSTANCE_ID=82b41977-1f13-4beb-b166-6b28a692d719
THEIA_WEBVIEW_EXTERNAL_ENDPOINT=webview-{{hostname}}
POETRY_CACHE_DIR=/workspace/.pyenv_mirror/poetry
NGINX_DOCROOT_IN_REPO=public
GITPOD_REPO_ROOTS=/workspace/aws-bootcamp-cruddur-2023
GOROOT=/home/gitpod/go
PIP_CACHE_DIR=/workspace/.pyenv_mirror/pip_cache
GITPOD_WORKSPACE_URL=https://burreetoman-awsbootcamp-81p8i5r1rli.ws-us92.gitpod.io
HOMEBREW_NO_AUTO_UPDATE=1
INFOPATH=:/home/linuxbrew/.linuxbrew/share/info
GITPOD_THEIA_PORT=23000
NVM_DIR=/home/gitpod/.nvm
GITPOD_WORKSPACE_CONTEXT={"isFile":false,"path":"","title":"burreetoman/aws-bootcamp-cruddur-2023 - main","ref":"main","refType":"branch","revision":"782a6201100f354c0267fe46f5e3428fb58548ac","repository":{"cloneUrl":"https://github.com/burreetoman/aws-bootcamp-cruddur-2023.git","host":"github.com","defaultBranch":"main","name":"aws-bootcamp-cruddur-2023","owner":"burreetoman","private":false},"normalizedContextURL":"https://github.com/burreetoman/aws-bootcamp-cruddur-2023","checkoutLocation":"aws-bootcamp-cruddur-2023"}
rvm_bin_path=/home/gitpod/.rvm/bin
GO_VERSION=1.19.5
GEM_PATH=/home/gitpod/.rvm/gems/ruby-3.1.2:/home/gitpod/.rvm/gems/ruby-3.1.2@global
GRADLE_USER_HOME=/workspace/.gradle/
GITPOD_CLI_APITOKEN=KETHZC1juw4eNsaAjZs74I90APNf2gCQ
GEM_HOME=/home/gitpod/.rvm/gems/ruby-3.1.2
LESSCLOSE=/usr/bin/lesspipe %s %s
TERM=xterm-256color
LESSOPEN=| /usr/bin/lesspipe %s
USER=gitpod
JAVA_TOOL_OPTIONS= -Xmx3489m
GITPOD_WORKSPACE_CLUSTER_HOST=ws-us92.gitpod.io
GITPOD_GIT_USER_NAME=burreetoman
MAVEN_HOME=/home/gitpod/.sdkman/candidates/maven/current
VISUAL=/ide/bin/remote-cli/gitpod-code
SDKMAN_DIR=/home/gitpod/.sdkman
AWS_ACCOUNT_ID=933248951695
SHLVL=1
GIT_EDITOR=/ide/bin/remote-cli/gitpod-code --wait
GITPOD_MEMORY=3489
AWS_ACCOUNT_IS=933248951695
AWS_ACCESS_KEY_ID=AKIA5SSPY4WHQQQMULX5
SDKMAN_CANDIDATES_API=https://api.sdkman.io/2
GITPOD_CONFIGCAT_ENABLED=true
PYENV_ROOT=/home/gitpod/.pyenv
GITPOD_ANALYTICS_SEGMENT_KEY=bUY8IRdJ42KjLOBS9LoIHMYFBD8rSzjU
GITPOD_HOST=https://gitpod.io
GITPOD_IDE_ALIAS=code
PATH=/home/gitpod/.sdkman/candidates/maven/current/bin:/home/gitpod/.sdkman/candidates/java/current/bin:/home/gitpod/.sdkman/candidates/gradle/current/bin:/workspace/.cargo/bin:/home/gitpod/.rvm/gems/ruby-3.1.2/bin:/home/gitpod/.rvm/gems/ruby-3.1.2@global/bin:/home/gitpod/.rvm/rubies/ruby-3.1.2/bin:/home/gitpod/.pyenv/shims:/workspace/go/bin:/home/gitpod/.nix-profile/bin:/ide/bin/remote-cli:/home/gitpod/go/bin:/home/gitpod/go-packages/bin:/home/gitpod/.nvm/versions/node/v16.19.0/bin:/home/gitpod/.yarn/bin:/home/gitpod/.pnpm:/home/gitpod/.pyenv/bin:/workspace/.rvm/bin:/home/gitpod/.cargo/bin:/home/linuxbrew/.linuxbrew/bin:/home/linuxbrew/.linuxbrew/sbin/:/home/gitpod/.local/bin:/usr/games:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/home/gitpod/.nvm/versions/node/v16.19.0/bin:/home/gitpod/.rvm/bin
PYTHONUSERBASE=/workspace/.pyenv_mirror/user/current
GP_PYENV_MIRROR=/workspace/.pyenv_mirror
SDKMAN_PLATFORM=linuxx64
APACHE_DOCROOT_IN_REPO=public
NODE_VERSION=16.19.0
GITPOD_GIT_USER_EMAIL=pdonner@truenollc.net
IRBRC=/home/gitpod/.rvm/rubies/ruby-3.1.2/.irbrc
VSX_REGISTRY_URL=https://open-vsx.gitpod.io
rvm_path=/home/gitpod/.rvm
GOPATH=/workspace/go
GITPOD_TASKS=[{"name":"aws-cli","env":{"AWS_CLI_AUTO_PROMPT":"on-partial"},"init":"cd /workspace\ncurl \"https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip\" -o \"awscliv2.zip\"\nunzip awscliv2.zip\nsudo ./aws/install\ncd $THEIA_WORKSPACE_ROOT\n"},{"name":"postgres","init":"curl -fsSL https://www.postgresql.org/media/keys/ACCC4CF8.asc|sudo gpg --dearmor -o /etc/apt/trusted.gpg.d/postgresql.gpg\necho \"deb http://apt.postgresql.org/pub/repos/apt/ `lsb_release -cs`-pgdg main\" |sudo tee  /etc/apt/sources.list.d/pgdg.list\nsudo apt update\nsudo apt install -y postgresql-client-13 libpq-dev\n"}]
_=/usr/bin/env
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ env | grep API
HONEYCOMB_API_KEY=ovnK5dcmiodHM75hiEFFmC
GITPOD_CLI_APITOKEN=KETHZC1juw4eNsaAjZs74I90APNf2gCQ
SDKMAN_CANDIDATES_API=https://api.sdkman.io/2
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ export HONEYCOMB_SERVICE_NAME="cruddur"
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ gp env HONEYCOMB_SERVICE_NAME="cruddur"
HONEYCOMB_SERVICE_NAME=cruddur
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ env | grep SERVICE_
HONEYCOMB_SERVICE_NAME=cruddur
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 


gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ pip install -r requirements.txt
ERROR: Could not open requirements file: [Errno 2] No such file or directory: 'requirements.txt'

[notice] A new release of pip available: 22.3.1 -> 23.0.1
[notice] To update, run: pip install --upgrade pip
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ pip install -r requirements.txt
ERROR: Could not open requirements file: [Errno 2] No such file or directory: 'requirements.txt'

[notice] A new release of pip available: 22.3.1 -> 23.0.1
[notice] To update, run: pip install --upgrade pip
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ cd backend-flask
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ pip install -r requirements.txt
Collecting flask
  Downloading Flask-2.2.3-py3-none-any.whl (101 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 101.8/101.8 kB 6.0 MB/s eta 0:00:00
Collecting flask-cors
  Downloading Flask_Cors-3.0.10-py2.py3-none-any.whl (14 kB)
Collecting opentelemetry-api
  Downloading opentelemetry_api-1.17.0-py3-none-any.whl (57 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 57.3/57.3 kB 23.7 MB/s eta 0:00:00
Collecting opentelemetry-sdk
  Downloading opentelemetry_sdk-1.17.0-py3-none-any.whl (100 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100.0/100.0 kB 36.5 MB/s eta 0:00:00
Collecting opentelemetry-exporter-otlp-proto-http
  Downloading opentelemetry_exporter_otlp_proto_http-1.17.0-py3-none-any.whl (21 kB)
Collecting opentelemetry-instrumentation-flask
  Downloading opentelemetry_instrumentation_flask-0.38b0-py3-none-any.whl (13 kB)
Collecting opentelemetry-instrumentation-requests
  Downloading opentelemetry_instrumentation_requests-0.38b0-py3-none-any.whl (11 kB)
Requirement already satisfied: Jinja2>=3.0 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from flask->-r requirements.txt (line 1)) (3.1.2)
Requirement already satisfied: importlib-metadata>=3.6.0 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from flask->-r requirements.txt (line 1)) (6.0.0)
Collecting itsdangerous>=2.0
  Downloading itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Collecting click>=8.0
  Downloading click-8.1.3-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.6/96.6 kB 30.9 MB/s eta 0:00:00
Collecting Werkzeug>=2.2.2
  Downloading Werkzeug-2.2.3-py3-none-any.whl (233 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 233.6/233.6 kB 64.3 MB/s eta 0:00:00
Requirement already satisfied: Six in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from flask-cors->-r requirements.txt (line 2)) (1.16.0)
Requirement already satisfied: setuptools>=16.0 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from opentelemetry-api->-r requirements.txt (line 4)) (65.6.3)
Collecting deprecated>=1.2.6
  Downloading Deprecated-1.2.13-py2.py3-none-any.whl (9.6 kB)
Collecting opentelemetry-semantic-conventions==0.38b0
  Downloading opentelemetry_semantic_conventions-0.38b0-py3-none-any.whl (26 kB)
Requirement already satisfied: typing-extensions>=3.7.4 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from opentelemetry-sdk->-r requirements.txt (line 5)) (4.4.0)
Collecting backoff<3.0.0,>=1.10.0
  Downloading backoff-2.2.1-py3-none-any.whl (15 kB)
Collecting googleapis-common-protos~=1.52
  Downloading googleapis_common_protos-1.59.0-py2.py3-none-any.whl (223 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 223.6/223.6 kB 71.0 MB/s eta 0:00:00
Collecting opentelemetry-proto==1.17.0
  Downloading opentelemetry_proto-1.17.0-py3-none-any.whl (52 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 52.6/52.6 kB 24.1 MB/s eta 0:00:00
Requirement already satisfied: requests~=2.7 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from opentelemetry-exporter-otlp-proto-http->-r requirements.txt (line 6)) (2.28.1)
Collecting protobuf<5.0,>=3.19
  Downloading protobuf-4.22.1-cp37-abi3-manylinux2014_x86_64.whl (302 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 302.4/302.4 kB 74.0 MB/s eta 0:00:00
Collecting opentelemetry-util-http==0.38b0
  Downloading opentelemetry_util_http-0.38b0-py3-none-any.whl (6.7 kB)
Collecting opentelemetry-instrumentation-wsgi==0.38b0
  Downloading opentelemetry_instrumentation_wsgi-0.38b0-py3-none-any.whl (12 kB)
Collecting opentelemetry-instrumentation==0.38b0
  Downloading opentelemetry_instrumentation-0.38b0-py3-none-any.whl (24 kB)
Requirement already satisfied: wrapt<2.0.0,>=1.0.0 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from opentelemetry-instrumentation==0.38b0->opentelemetry-instrumentation-flask->-r requirements.txt (line 7)) (1.14.1)
Requirement already satisfied: zipp>=0.5 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from importlib-metadata>=3.6.0->flask->-r requirements.txt (line 1)) (3.11.0)
Requirement already satisfied: MarkupSafe>=2.0 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from Jinja2>=3.0->flask->-r requirements.txt (line 1)) (2.1.1)
Requirement already satisfied: urllib3<1.27,>=1.21.1 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from requests~=2.7->opentelemetry-exporter-otlp-proto-http->-r requirements.txt (line 6)) (1.26.13)
Requirement already satisfied: certifi>=2017.4.17 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from requests~=2.7->opentelemetry-exporter-otlp-proto-http->-r requirements.txt (line 6)) (2022.12.7)
Requirement already satisfied: idna<4,>=2.5 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from requests~=2.7->opentelemetry-exporter-otlp-proto-http->-r requirements.txt (line 6)) (3.4)
Requirement already satisfied: charset-normalizer<3,>=2 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from requests~=2.7->opentelemetry-exporter-otlp-proto-http->-r requirements.txt (line 6)) (2.1.1)
Installing collected packages: Werkzeug, protobuf, opentelemetry-util-http, opentelemetry-semantic-conventions, itsdangerous, deprecated, click, backoff, opentelemetry-proto, opentelemetry-api, googleapis-common-protos, flask, opentelemetry-sdk, opentelemetry-instrumentation, flask-cors, opentelemetry-instrumentation-wsgi, opentelemetry-instrumentation-requests, opentelemetry-exporter-otlp-proto-http, opentelemetry-instrumentation-flask
Successfully installed Werkzeug-2.2.3 backoff-2.2.1 click-8.1.3 deprecated-1.2.13 flask-2.2.3 flask-cors-3.0.10 googleapis-common-protos-1.59.0 itsdangerous-2.1.2 opentelemetry-api-1.17.0 opentelemetry-exporter-otlp-proto-http-1.17.0 opentelemetry-instrumentation-0.38b0 opentelemetry-instrumentation-flask-0.38b0 opentelemetry-instrumentation-requests-0.38b0 opentelemetry-instrumentation-wsgi-0.38b0 opentelemetry-proto-1.17.0 opentelemetry-sdk-1.17.0 opentelemetry-semantic-conventions-0.38b0 opentelemetry-util-http-0.38b0 protobuf-4.22.1

[notice] A new release of pip available: 22.3.1 -> 23.0.1
[notice] To update, run: pip install --upgrade pip
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ 

# ===============
# RUN NPM INSTALL
# ===============

gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ pip install -r requirements.txt
ERROR: Could not open requirements file: [Errno 2] No such file or directory: 'requirements.txt'

[notice] A new release of pip available: 22.3.1 -> 23.0.1
[notice] To update, run: pip install --upgrade pip
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ pip install -r requirements.txt
ERROR: Could not open requirements file: [Errno 2] No such file or directory: 'requirements.txt'

[notice] A new release of pip available: 22.3.1 -> 23.0.1
[notice] To update, run: pip install --upgrade pip
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ cd backend-flask
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ pip install -r requirements.txt
Collecting flask
  Downloading Flask-2.2.3-py3-none-any.whl (101 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 101.8/101.8 kB 6.0 MB/s eta 0:00:00
Collecting flask-cors
  Downloading Flask_Cors-3.0.10-py2.py3-none-any.whl (14 kB)
Collecting opentelemetry-api
  Downloading opentelemetry_api-1.17.0-py3-none-any.whl (57 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 57.3/57.3 kB 23.7 MB/s eta 0:00:00
Collecting opentelemetry-sdk
  Downloading opentelemetry_sdk-1.17.0-py3-none-any.whl (100 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100.0/100.0 kB 36.5 MB/s eta 0:00:00
Collecting opentelemetry-exporter-otlp-proto-http
  Downloading opentelemetry_exporter_otlp_proto_http-1.17.0-py3-none-any.whl (21 kB)
Collecting opentelemetry-instrumentation-flask
  Downloading opentelemetry_instrumentation_flask-0.38b0-py3-none-any.whl (13 kB)
Collecting opentelemetry-instrumentation-requests
  Downloading opentelemetry_instrumentation_requests-0.38b0-py3-none-any.whl (11 kB)
Requirement already satisfied: Jinja2>=3.0 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from flask->-r requirements.txt (line 1)) (3.1.2)
Requirement already satisfied: importlib-metadata>=3.6.0 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from flask->-r requirements.txt (line 1)) (6.0.0)
Collecting itsdangerous>=2.0
  Downloading itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Collecting click>=8.0
  Downloading click-8.1.3-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.6/96.6 kB 30.9 MB/s eta 0:00:00
Collecting Werkzeug>=2.2.2
  Downloading Werkzeug-2.2.3-py3-none-any.whl (233 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 233.6/233.6 kB 64.3 MB/s eta 0:00:00
Requirement already satisfied: Six in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from flask-cors->-r requirements.txt (line 2)) (1.16.0)
Requirement already satisfied: setuptools>=16.0 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from opentelemetry-api->-r requirements.txt (line 4)) (65.6.3)
Collecting deprecated>=1.2.6
  Downloading Deprecated-1.2.13-py2.py3-none-any.whl (9.6 kB)
Collecting opentelemetry-semantic-conventions==0.38b0
  Downloading opentelemetry_semantic_conventions-0.38b0-py3-none-any.whl (26 kB)
Requirement already satisfied: typing-extensions>=3.7.4 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from opentelemetry-sdk->-r requirements.txt (line 5)) (4.4.0)
Collecting backoff<3.0.0,>=1.10.0
  Downloading backoff-2.2.1-py3-none-any.whl (15 kB)
Collecting googleapis-common-protos~=1.52
  Downloading googleapis_common_protos-1.59.0-py2.py3-none-any.whl (223 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 223.6/223.6 kB 71.0 MB/s eta 0:00:00
Collecting opentelemetry-proto==1.17.0
  Downloading opentelemetry_proto-1.17.0-py3-none-any.whl (52 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 52.6/52.6 kB 24.1 MB/s eta 0:00:00
Requirement already satisfied: requests~=2.7 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from opentelemetry-exporter-otlp-proto-http->-r requirements.txt (line 6)) (2.28.1)
Collecting protobuf<5.0,>=3.19
  Downloading protobuf-4.22.1-cp37-abi3-manylinux2014_x86_64.whl (302 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 302.4/302.4 kB 74.0 MB/s eta 0:00:00
Collecting opentelemetry-util-http==0.38b0
  Downloading opentelemetry_util_http-0.38b0-py3-none-any.whl (6.7 kB)
Collecting opentelemetry-instrumentation-wsgi==0.38b0
  Downloading opentelemetry_instrumentation_wsgi-0.38b0-py3-none-any.whl (12 kB)
Collecting opentelemetry-instrumentation==0.38b0
  Downloading opentelemetry_instrumentation-0.38b0-py3-none-any.whl (24 kB)
Requirement already satisfied: wrapt<2.0.0,>=1.0.0 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from opentelemetry-instrumentation==0.38b0->opentelemetry-instrumentation-flask->-r requirements.txt (line 7)) (1.14.1)
Requirement already satisfied: zipp>=0.5 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from importlib-metadata>=3.6.0->flask->-r requirements.txt (line 1)) (3.11.0)
Requirement already satisfied: MarkupSafe>=2.0 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from Jinja2>=3.0->flask->-r requirements.txt (line 1)) (2.1.1)
Requirement already satisfied: urllib3<1.27,>=1.21.1 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from requests~=2.7->opentelemetry-exporter-otlp-proto-http->-r requirements.txt (line 6)) (1.26.13)
Requirement already satisfied: certifi>=2017.4.17 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from requests~=2.7->opentelemetry-exporter-otlp-proto-http->-r requirements.txt (line 6)) (2022.12.7)
Requirement already satisfied: idna<4,>=2.5 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from requests~=2.7->opentelemetry-exporter-otlp-proto-http->-r requirements.txt (line 6)) (3.4)
Requirement already satisfied: charset-normalizer<3,>=2 in /home/gitpod/.pyenv/versions/3.8.16/lib/python3.8/site-packages (from requests~=2.7->opentelemetry-exporter-otlp-proto-http->-r requirements.txt (line 6)) (2.1.1)
Installing collected packages: Werkzeug, protobuf, opentelemetry-util-http, opentelemetry-semantic-conventions, itsdangerous, deprecated, click, backoff, opentelemetry-proto, opentelemetry-api, googleapis-common-protos, flask, opentelemetry-sdk, opentelemetry-instrumentation, flask-cors, opentelemetry-instrumentation-wsgi, opentelemetry-instrumentation-requests, opentelemetry-exporter-otlp-proto-http, opentelemetry-instrumentation-flask
Successfully installed Werkzeug-2.2.3 backoff-2.2.1 click-8.1.3 deprecated-1.2.13 flask-2.2.3 flask-cors-3.0.10 googleapis-common-protos-1.59.0 itsdangerous-2.1.2 opentelemetry-api-1.17.0 opentelemetry-exporter-otlp-proto-http-1.17.0 opentelemetry-instrumentation-0.38b0 opentelemetry-instrumentation-flask-0.38b0 opentelemetry-instrumentation-requests-0.38b0 opentelemetry-instrumentation-wsgi-0.38b0 opentelemetry-proto-1.17.0 opentelemetry-sdk-1.17.0 opentelemetry-semantic-conventions-0.38b0 opentelemetry-util-http-0.38b0 protobuf-4.22.1

[notice] A new release of pip available: 22.3.1 -> 23.0.1
[notice] To update, run: pip install --upgrade pip
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ 
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ 
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ npm i
npm ERR! code ENOENT
npm ERR! syscall open
npm ERR! path /workspace/aws-bootcamp-cruddur-2023/backend-flask/package.json
npm ERR! errno -2
npm ERR! enoent ENOENT: no such file or directory, open '/workspace/aws-bootcamp-cruddur-2023/backend-flask/package.json'
npm ERR! enoent This is related to npm not being able to find a file.
npm ERR! enoent 

npm ERR! A complete log of this run can be found in:
npm ERR!     /home/gitpod/.npm/_logs/2023-03-25T00_47_18_488Z-debug-0.log
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ cd ../frontend-react
bash: cd: ../frontend-react: No such file or directory
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ npm i
npm ERR! code ENOENT
npm ERR! syscall open
npm ERR! path /workspace/aws-bootcamp-cruddur-2023/backend-flask/package.json
npm ERR! errno -2
npm ERR! enoent ENOENT: no such file or directory, open '/workspace/aws-bootcamp-cruddur-2023/backend-flask/package.json'
npm ERR! enoent This is related to npm not being able to find a file.
npm ERR! enoent 

npm ERR! A complete log of this run can be found in:
npm ERR!     /home/gitpod/.npm/_logs/2023-03-25T00_47_50_581Z-debug-0.log
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ cd frontend-react
bash: cd: frontend-react: No such file or directory
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ cd frontend-react.js
bash: cd: frontend-react.js: No such file or directory
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ cd frontend-react-js
bash: cd: frontend-react-js: No such file or directory
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ npm i
npm ERR! code ENOENT
npm ERR! syscall open
npm ERR! path /workspace/aws-bootcamp-cruddur-2023/backend-flask/package.json
npm ERR! errno -2
npm ERR! enoent ENOENT: no such file or directory, open '/workspace/aws-bootcamp-cruddur-2023/backend-flask/package.json'
npm ERR! enoent This is related to npm not being able to find a file.
npm ERR! enoent 

npm ERR! A complete log of this run can be found in:
npm ERR!     /home/gitpod/.npm/_logs/2023-03-25T00_49_53_437Z-debug-0.log
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ pwd
/workspace/aws-bootcamp-cruddur-2023/backend-flask
gitpod /workspace/aws-bootcamp-cruddur-2023/backend-flask (main) $ cd ../frontend-react-js
gitpod /workspace/aws-bootcamp-cruddur-2023/frontend-react-js (main) $ npm i
(#########⠂⠂⠂⠂⠂⠂⠂⠂⠂) ⠹ reify:negotiator: timing reifyNode:node_modules/string-width/node_modules/emoji-regex Complet(#########⠂⠂⠂⠂⠂⠂⠂⠂⠂) ⠹ reify:negotiator: timing reifyNode:node_modules/string-width/node_modules/emoji-regex Complet(#########⠂⠂⠂⠂⠂⠂⠂⠂⠂) ⠹ reify:negotiator: timing reifyNode:node_modules/string-width/node_modules/emoji-regex Complet(#########⠂⠂⠂⠂⠂⠂⠂⠂⠂) ⠸ reify:wrap-ansi: http fetch GET 200 https://registry.npmjs.org/wrap-ansi/-/wrap-ansi-7.0.0.tg(#########⠂⠂⠂⠂⠂⠂⠂⠂⠂) ⠴ reify:y18n: http fetch GET 200 https://registry.npmjs.org/y18n/-/y18n-5.0.8.tgz 4318ms (cache(#########⠂⠂⠂⠂⠂⠂⠂⠂⠂) ⠧ reify:word-wrap: http fetch GET 200 https://registry.npmjs.org/word-wrap/-/word-wrap-1.2.3.tg(#########⠂⠂⠂⠂⠂⠂⠂⠂⠂) ⠋ reify:vary: http fetch GET 200 https://registry.npmjs.org/vary/-/vary-1.1.2.tgz 4387ms (cache
npm WARN deprecated w3c-hr-time@1.0.2: Use your platform's native performance.now() and performance.timeOrigin.
(#########⠂⠂⠂⠂⠂⠂⠂⠂⠂) ⠙ reify:w3c-hr-time: WARN deprecated w3c-hr-time@1.0.2: Use your platform's native performance.(#########⠂⠂⠂⠂⠂⠂⠂⠂⠂) ⠴ reify:walker: http fetch GET 200 https://registry.npmjs.org/walker/-/walker-1.0.8.tgz 4507ms (#########⠂⠂⠂⠂⠂⠂⠂⠂⠂) ⠦ reify:type-check: http fetch GET 200 https://registry.npmjs.org/type-check/-/type-check-0.4.0(#########⠂⠂⠂⠂⠂⠂⠂⠂⠂) ⠸ reify:throat: http fetch GET 200 https://registry.npmjs.org/throat/-/throat-6.0.2.tgz 4580ms (##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠇ reify:tempy: http fetch GET 200 https://registry.npmjs.org/tempy/-/tempy-0.6.0.tgz 4635ms (ca(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠇ reify:supports-hyperlinks: http fetch GET 200 https://registry.npmjs.org/supports-hyperlinks/(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠼ reify:strip-indent: http fetch GET 200 https://registry.npmjs.org/strip-indent/-/strip-indent(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠹ reify:unicode-match-property-ecmascript: http fetch GET 200 https://registry.npmjs.org/unicod(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠋ reify:string-length: http fetch GET 200 https://registry.npmjs.org/string-length/-/string-len(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠏ reify:strip-final-newline: http fetch GET 200 https://registry.npmjs.org/strip-final-newline/(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠙ reify:slash: http fetch GET 200 https://registry.npmjs.org/slash/-/slash-3.0.0.tgz 5032ms (ca
npm WARN deprecated stable@0.1.8: Modern JS already guarantees Array#sort() is a stable sort, so this library is deprecated. See the compatibility table on MDN: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort#browser_compatibility
(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠙ reify:selfsigned: http fetch GET 200 https://registry.npmjs.org/selfsigned/-/selfsigned-2.1.1
npm WARN deprecated sourcemap-codec@1.4.8: Please use @jridgewell/sourcemap-codec instead
npm WARN deprecated rollup-plugin-terser@7.0.2: This package has been deprecated and is no longer maintained. Please use @rollup/plugin-terser
(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠴ reify:run-parallel: http fetch GET 200 https://registry.npmjs.org/run-parallel/-/run-parallel(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠏ reify:require-from-string: http fetch GET 200 https://registry.npmjs.org/require-from-string/(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠇ reify:safe-regex-test: http fetch GET 200 https://registry.npmjs.org/safe-regex-test/-/safe-r(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠧ reify:readdirp: http fetch GET 200 https://registry.npmjs.org/readdirp/-/readdirp-3.6.0.tgz 5(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠋ reify:require-directory: http fetch GET 200 https://registry.npmjs.org/require-directory/-/re(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠇ reify:randombytes: http fetch GET 200 https://registry.npmjs.org/randombytes/-/randombytes-2.(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠏ reify:querystringify: http fetch GET 200 https://registry.npmjs.org/querystringify/-/querystr(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠹ reify:pretty-bytes: http fetch GET 200 https://registry.npmjs.org/pretty-bytes/-/pretty-bytes(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠹ reify:postcss-pseudo-class-any-link: http fetch GET 200 https://registry.npmjs.org/postcss-ps(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠹ reify:postcss-normalize-url: http fetch GET 200 https://registry.npmjs.org/postcss-normalize-(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠦ reify:postcss-normalize-positions: http fetch GET 200 https://registry.npmjs.org/postcss-norm(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠇ reify:postcss-normalize: http fetch GET 200 https://registry.npmjs.org/postcss-normalize/-/po(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠹ reify:postcss-minify-params: http fetch GET 200 https://registry.npmjs.org/postcss-minify-par(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠙ reify:postcss-import: http fetch GET 200 https://registry.npmjs.org/postcss-import/-/postcss-(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠦ reify:postcss-discard-empty: http fetch GET 200 https://registry.npmjs.org/postcss-discard-em(##########⠂⠂⠂⠂⠂⠂⠂⠂) ⠦ reify:postcss-custom-selectors: http fetch GET 200 https://registry.npmjs.org/postcss-custom-(###########⠂⠂⠂⠂⠂⠂⠂) ⠙ reify:pkg-dir: http fetch GET 200 https://registry.npmjs.org/pkg-dir/-/pkg-dir-4.2.0.tgz 6605(###########⠂⠂⠂⠂⠂⠂⠂) ⠏ reify:path-key: http fetch GET 200 https://registry.npmjs.org/path-key/-/path-key-3.1.1.tgz 6(###########⠂⠂⠂⠂⠂⠂⠂) ⠴ reify:p-try: http fetch GET 200 https://registry.npmjs.org/p-try/-/p-try-2.2.0.tgz 6718ms (ca(###########⠂⠂⠂⠂⠂⠂⠂) ⠏ reify:on-headers: http fetch GET 200 https://registry.npmjs.org/on-headers/-/on-headers-1.0.2(###########⠂⠂⠂⠂⠂⠂⠂) ⠧ reify:on-finished: http fetch GET 200 https://registry.npmjs.org/on-finished/-/on-finished-2.(###########⠂⠂⠂⠂⠂⠂⠂) ⠇ reify:multicast-dns: http fetch GET 200 https://registry.npmjs.org/multicast-dns/-/multicast-(###########⠂⠂⠂⠂⠂⠂⠂) ⠦ reify:micromatch: http fetch GET 200 https://registry.npmjs.org/micromatch/-/micromatch-4.0.5(###########⠂⠂⠂⠂⠂⠂⠂) ⠙ reify:lru-cache: http fetch GET 200 https://registry.npmjs.org/lru-cache/-/lru-cache-5.1.1.tg(###########⠂⠂⠂⠂⠂⠂⠂) ⠦ reify:lodash.memoize: http fetch GET 200 https://registry.npmjs.org/lodash.memoize/-/lodash.m(###########⠂⠂⠂⠂⠂⠂⠂) ⠋ reify:leven: http fetch GET 200 https://registry.npmjs.org/leven/-/leven-3.1.0.tgz 7168ms (ca(###########⠂⠂⠂⠂⠂⠂⠂) ⠏ reify:merge-stream: http fetch GET 200 https://registry.npmjs.org/merge-stream/-/merge-stream(###########⠂⠂⠂⠂⠂⠂⠂) ⠴ reify:json-parse-even-better-errors: http fetch GET 200 https://registry.npmjs.org/json-parse(###########⠂⠂⠂⠂⠂⠂⠂) ⠋ reify:js-cookie: http fetch GET 200 https://registry.npmjs.org/js-cookie/-/js-cookie-3.0.1.tg(###########⠂⠂⠂⠂⠂⠂⠂) ⠹ reify:jest-resolve-dependencies: http fetch GET 200 https://registry.npmjs.org/jest-resolve-d(###########⠂⠂⠂⠂⠂⠂⠂) ⠹ reify:jest-pnp-resolver: http fetch GET 200 https://registry.npmjs.org/jest-pnp-resolver/-/je(###########⠂⠂⠂⠂⠂⠂⠂) ⠸ reify:jest-pnp-resolver: http fetch GET 200 https://registry.npmjs.org/jest-pnp-resolver/-/je(###########⠂⠂⠂⠂⠂⠂⠂) ⠴ reify:jest-docblock: http fetch GET 200 https://registry.npmjs.org/jest-docblock/-/jest-docbl(###########⠂⠂⠂⠂⠂⠂⠂) ⠼ reify:is-wsl: http fetch GET 200 https://registry.npmjs.org/is-wsl/-/is-wsl-2.2.0.tgz 7624ms (###########⠂⠂⠂⠂⠂⠂⠂) ⠇ reify:is-typedarray: http fetch GET 200 https://registry.npmjs.org/is-typedarray/-/is-typedar(###########⠂⠂⠂⠂⠂⠂⠂) ⠹ reify:is-obj: http fetch GET 200 https://registry.npmjs.org/is-obj/-/is-obj-1.0.1.tgz 7766ms (############⠂⠂⠂⠂⠂⠂) ⠏ reify:is-generator-fn: http fetch GET 200 https://registry.npmjs.org/is-generator-fn/-/is-gen(############⠂⠂⠂⠂⠂⠂) ⠇ reify:is-arrayish: http fetch GET 200 https://registry.npmjs.org/is-arrayish/-/is-arrayish-0.(############⠂⠂⠂⠂⠂⠂) ⠼ reify:import-local: http fetch GET 200 https://registry.npmjs.org/import-local/-/import-local(############⠂⠂⠂⠂⠂⠂) ⠸ reify:ignore: http fetch GET 200 https://registry.npmjs.org/ignore/-/ignore-5.2.4.tgz 7977ms (############⠂⠂⠂⠂⠂⠂) ⠇ reify:http-parser-js: http fetch GET 200 https://registry.npmjs.org/http-parser-js/-/http-par(############⠂⠂⠂⠂⠂⠂) ⠸ reify:html-encoding-sniffer: http fetch GET 200 https://registry.npmjs.org/html-encoding-snif(############⠂⠂⠂⠂⠂⠂) ⠙ reify:has: http fetch GET 200 https://registry.npmjs.org/has/-/has-1.0.3.tgz 8134ms (cache mi(############⠂⠂⠂⠂⠂⠂) ⠇ reify:global-prefix: http fetch GET 200 https://registry.npmjs.org/global-prefix/-/global-pre(############⠂⠂⠂⠂⠂⠂) ⠸ reify:get-package-type: http fetch GET 200 https://registry.npmjs.org/get-package-type/-/get-(############⠂⠂⠂⠂⠂⠂) ⠇ reify:follow-redirects: http fetch GET 200 https://registry.npmjs.org/follow-redirects/-/foll(############⠂⠂⠂⠂⠂⠂) ⠦ reify:fb-watchman: http fetch GET 200 https://registry.npmjs.org/fb-watchman/-/fb-watchman-2.(############⠂⠂⠂⠂⠂⠂) ⠋ reify:esrecurse: http fetch GET 200 https://registry.npmjs.org/esrecurse/-/esrecurse-4.3.0.tg(############⠂⠂⠂⠂⠂⠂) ⠏ reify:estraverse: http fetch GET 200 https://registry.npmjs.org/estraverse/-/estraverse-5.3.0(############⠂⠂⠂⠂⠂⠂) ⠦ reify:es-set-tostringtag: http fetch GET 200 https://registry.npmjs.org/es-set-tostringtag/-/(############⠂⠂⠂⠂⠂⠂) ⠇ reify:emittery: http fetch GET 200 https://registry.npmjs.org/emittery/-/emittery-0.8.1.tgz 8(############⠂⠂⠂⠂⠂⠂) ⠙ reify:escape-html: http fetch GET 200 https://registry.npmjs.org/escape-html/-/escape-html-1.(############⠂⠂⠂⠂⠂⠂) ⠙ reify:dir-glob: http fetch GET 200 https://registry.npmjs.org/dir-glob/-/dir-glob-3.0.1.tgz 8(#############⠂⠂⠂⠂⠂) ⠴ reify:detect-node: http fetch GET 200 https://registry.npmjs.org/detect-node/-/detect-node-2.(#############⠂⠂⠂⠂⠂) ⠼ reify:data-urls: http fetch GET 200 https://registry.npmjs.org/data-urls/-/data-urls-2.0.0.tg(#############⠂⠂⠂⠂⠂) ⠏ reify:css-select-base-adapter: http fetch GET 200 https://registry.npmjs.org/css-select-base-(#############⠂⠂⠂⠂⠂) ⠴ reify:connect-history-api-fallback: http fetch GET 200 https://registry.npmjs.org/connect-his(#############⠂⠂⠂⠂⠂) ⠹ reify:combined-stream: http fetch GET 200 https://registry.npmjs.org/combined-stream/-/combin(#############⠂⠂⠂⠂⠂) ⠋ reify:collect-v8-coverage: http fetch GET 200 https://registry.npmjs.org/collect-v8-coverage/(#############⠂⠂⠂⠂⠂) ⠦ reify:char-regex: http fetch GET 200 https://registry.npmjs.org/char-regex/-/char-regex-1.0.2(#############⠂⠂⠂⠂⠂) ⠼ reify:bser: http fetch GET 200 https://registry.npmjs.org/bser/-/bser-2.1.1.tgz 9336ms (cache(#############⠂⠂⠂⠂⠂) ⠇ reify:batch: http fetch GET 200 https://registry.npmjs.org/batch/-/batch-0.6.1.tgz 9372ms (ca(#############⠂⠂⠂⠂⠂) ⠸ reify:babel-plugin-polyfill-regenerator: http fetch GET 200 https://registry.npmjs.org/babel-(#############⠂⠂⠂⠂⠂) ⠋ reify:ast-types-flow: http fetch GET 200 https://registry.npmjs.org/ast-types-flow/-/ast-type(#############⠂⠂⠂⠂⠂) ⠋ reify:ansi-html-community: http fetch GET 200 https://registry.npmjs.org/ansi-html-community/(#############⠂⠂⠂⠂⠂) ⠏ reify:abab: http fetch GET 200 https://registry.npmjs.org/abab/-/abab-2.0.6.tgz 9598ms (cache(#############⠂⠂⠂⠂⠂) ⠸ reify:@webassemblyjs/helper-wasm-bytecode: http fetch GET 200 https://registry.npmjs.org/@web(##############⠂⠂⠂⠂) ⠋ reify:@types/ws: http fetch GET 200 https://registry.npmjs.org/@types/ws/-/ws-8.5.4.tgz 9625m(##############⠂⠂⠂⠂) ⠸ reify:@types/range-parser: http fetch GET 200 https://registry.npmjs.org/@types/range-parser/(##############⠂⠂⠂⠂) ⠴ reify:@types/eslint-scope: http fetch GET 200 https://registry.npmjs.org/@types/eslint-scope/(##############⠂⠂⠂⠂) ⠹ reify:@tootallnate/once: http fetch GET 200 https://registry.npmjs.org/@tootallnate/once/-/on(##############⠂⠂⠂⠂) ⠹ reify:@svgr/babel-plugin-svg-em-dimensions: http fetch GET 200 https://registry.npmjs.org/@sv(##############⠂⠂⠂⠂) ⠇ reify:@svgr/babel-plugin-remove-jsx-empty-expression: http fetch GET 200 https://registry.npm(##############⠂⠂⠂⠂) ⠧ reify:@jridgewell/set-array: http fetch GET 200 https://registry.npmjs.org/@jridgewell/set-ar(##############⠂⠂⠂⠂) ⠴ reify:@jest/test-result: http fetch GET 200 https://registry.npmjs.org/@jest/test-result/-/te(##############⠂⠂⠂⠂) ⠹ reify:@istanbuljs/load-nyc-config: http fetch GET 200 https://registry.npmjs.org/@istanbuljs/(##############⠂⠂⠂⠂) ⠋ reify:@csstools/postcss-stepped-value-functions: http fetch GET 200 https://registry.npmjs.or(##############⠂⠂⠂⠂) ⠏ reify:@csstools/normalize.css: http fetch GET 200 https://registry.npmjs.org/@csstools/normal(##############⠂⠂⠂⠂) ⠧ reify:@babel/plugin-transform-template-literals: http fetch GET 200 https://registry.npmjs.or(##############⠂⠂⠂⠂) ⠸ reify:@babel/plugin-transform-modules-systemjs: http fetch GET 200 https://registry.npmjs.org(###############⠂⠂⠂) ⠦ reify:@babel/plugin-transform-block-scoped-functions: http fetch GET 200 https://registry.npm(###############⠂⠂⠂) ⠧ reify:@babel/plugin-syntax-private-property-in-object: http fetch GET 200 https://registry.np
npm WARN deprecated svgo@1.3.2: This SVGO version is no longer supported. Upgrade to v2.x.x.
(###############⠂⠂⠂) ⠴ reify:@jridgewell/trace-mapping: timing reifyNode:node_modules/enhanced-resolve Completed in (###############⠂⠂⠂) ⠴ reify:acorn: http fetch GET 200 https://registry.npmjs.org/acorn/-/acorn-8.8.2.tgz 10996ms (c(###############⠂⠂⠂) ⠹ reify:@csstools/postcss-oklab-function: timing reifyNode:node_modules/eslint-plugin-testing-l(###############⠂⠂⠂) ⠧ reify:@babel/plugin-transform-runtime: timing reifyNode:node_modules/@babel/plugin-transform-(###############⠂⠂⠂) ⠦ reify:@babel/helper-function-name: http fetch GET 200 https://registry.npmjs.org/@babel/helpe(###############⠂⠂⠂) ⠹ reify:@csstools/postcss-color-function: http fetch GET 200 https://registry.npmjs.org/@eslint(###############⠂⠂⠂) ⠴ reify:@eslint-community/eslint-utils: timing reifyNode:node_modules/@eslint-community/regexpp(###############⠂⠂⠂) ⠴ reify:@testing-library/jest-dom: timing reifyNode:node_modules/@types/semver Completed in 134(###############⠂⠂⠂) ⠋ reify:has-flag: http fetch GET 200 https://registry.npmjs.org/has-flag/-/has-flag-4.0.0.tgz 1(###############⠂⠂⠂) ⠧ reify:picocolors: http fetch GET 200 https://registry.npmjs.org/picocolors/-/picocolors-0.2.1(###############⠂⠂⠂) ⠦ reify:react-is: http fetch GET 200 https://registry.npmjs.org/react-is/-/react-is-16.13.1.tgz(###############⠂⠂⠂) ⠙ reify:locate-path: http fetch GET 200 https://registry.npmjs.org/locate-path/-/locate-path-5.(################⠂⠂) ⠴ reify:string-length: http fetch GET 200 https://registry.npmjs.org/string-length/-/string-len(################⠂⠂) ⠦ reify:emittery: http fetch GET 200 https://registry.npmjs.org/emittery/-/emittery-0.10.2.tgz (################⠂⠂) ⠋ reify:@jest/test-result: http fetch GET 200 https://registry.npmjs.org/@jest/test-result/-/te(################⠂⠂) ⠴ reify:color-convert: http fetch GET 200 https://registry.npmjs.org/color-convert/-/color-conv(################⠂⠂) ⠋ reify:has-flag: http fetch GET 200 https://registry.npmjs.org/has-flag/-/has-flag-4.0.0.tgz 1(################⠂⠂) ⠦ reify:color-convert: http fetch GET 200 https://registry.npmjs.org/color-convert/-/color-conv(################⠂⠂) ⠇ reify:color-name: http fetch GET 200 https://registry.npmjs.org/color-name/-/color-name-1.1.4(################⠂⠂) ⠙ reify:color-name: http fetch GET 200 https://registry.npmjs.org/color-name/-/color-name-1.1.4(################⠂⠂) ⠇ reify:color-name: http fetch GET 200 https://registry.npmjs.org/color-name/-/color-name-1.1.4(################⠂⠂) ⠼ reify:chalk: http fetch GET 200 https://registry.npmjs.org/chalk/-/chalk-4.1.2.tgz 11798ms (c(#################⠂) ⠧ reify:has-flag: http fetch GET 200 https://registry.npmjs.org/has-flag/-/has-flag-4.0.0.tgz 1(#################⠂) ⠼ reify:globals: http fetch GET 200 https://registry.npmjs.org/globals/-/globals-13.20.0.tgz 11(#################⠂) ⠏ reify:webidl-conversions: http fetch GET 200 https://registry.npmjs.org/webidl-conversions/-/(#################⠂) ⠦ reify:ms: http fetch GET 200 https://registry.npmjs.org/ms/-/ms-2.0.0.tgz 12075ms (cache miss(#################⠂) ⠇ reify:color-convert: http fetch GET 200 https://registry.npmjs.org/color-convert/-/color-conv(#################⠂) ⠦ reify:supports-color: http fetch GET 200 https://registry.npmjs.org/supports-color/-/supports(#################⠂) ⠋ reify:color-convert: http fetch GET 200 https://registry.npmjs.org/color-convert/-/color-conv(#################⠂) ⠧ reify:has-flag: http fetch GET 200 https://registry.npmjs.org/has-flag/-/has-flag-4.0.0.tgz 1(#################⠂) ⠇ reify:globals: http fetch GET 200 https://registry.npmjs.org/globals/-/globals-13.20.0.tgz 12(#################⠂) ⠦ reify:schema-utils: timing reifyNode:node_modules/fork-ts-checker-webpack-plugin/node_modules(#################⠂) ⠴ reify:@babel/helpers: timing reifyNode:node_modules/@types/jest/node_modules/jest-util Comple(#################⠂) ⠦ reify:mdn-data: timing reifyNode:node_modules/@jridgewell/source-map/node_modules/@jridgewell(#################⠂) ⠋ reify:@bcoe/v8-coverage: timing reifyNode:node_modules/@pmmmwh/react-refresh-webpack-plugin C(#################⠂) ⠼ reify:workbox-build: http fetch GET 200 https://registry.npmjs.org/workbox-build/-/workbox-bu(##################) ⠴ reify:source-map: http fetch GET 200 https://registry.npmjs.org/source-map/-/source-map-0.6.1(##################) ⠹ reify:fs-extra: http fetch GET 200 https://registry.npmjs.org/fs-extra/-/fs-extra-9.1.0.tgz 1(##################) ⠹ reify:mdn-data: http fetch GET 200 https://registry.npmjs.org/@babel/traverse/-/traverse-7.21(##################) ⠸ reify:@remix-run/router: http fetch GET 200 https://registry.npmjs.org/@remix-run/router/-/ro(##################) ⠇ reify:source-map: http fetch GET 200 https://registry.npmjs.org/source-map/-/source-map-0.6.1(##################) ⠏ reify:source-map: http fetch GET 200 https://registry.npmjs.org/source-map/-/source-map-0.6.1(##################) ⠋ reify:source-map: http fetch GET 200 https://registry.npmjs.org/source-map/-/source-map-0.6.1(##################) ⠧ reify:acorn: timing reifyNode:node_modules/acorn-globals/node_modules/acorn Completed in 1603(##################) ⠴ reify:clean-css: http fetch GET 200 https://registry.npmjs.org/clean-css/-/clean-css-5.3.2.tg(##################) ⠋ reify:eslint-plugin-import: http fetch GET 200 https://registry.npmjs.org/eslint-plugin-impor(##################) ⠼ reify:eslint-plugin-react: http fetch GET 200 https://registry.npmjs.org/eslint-plugin-react/(##################) ⠦ reify:svgo: http fetch GET 200 https://registry.npmjs.org/svgo/-/svgo-2.8.0.tgz 13653ms (cach(##################) ⠋ reify:ajv-keywords: timing reifyNode:node_modules/webpack-dev-server/node_modules/ajv-keyword(##################) ⠴ reify:ajv-keywords: http fetch GET 200 https://registry.npmjs.org/@typescript-eslint/typescri(##################) ⠋ reify:@typescript-eslint/typescript-estree: timing reifyNode:node_modules/mini-css-extract-pl(##################) ⠹ reify:css-tree: http fetch GET 200 https://registry.npmjs.org/css-tree/-/css-tree-1.0.0-alpha(##################) ⠋ reify:ajv-keywords: timing metavuln:calculate:security-advisory:@svgr/plugin-svgo:H4LeLrB8NCw(##################) ⠹ reify:ajv-keywords: timing metavuln:calculate:security-advisory:@svgr/plugin-svgo:H4LeLrB8NCw(##################) ⠧ reify:luxon: timing metavuln:load:security-advisory:@svgr/webpack:f/0iKu9ag0jtIunruFfqDrgnf9K(##################) ⠏ reify:resolve: http fetch GET 200 https://registry.npmjs.org/resolve/-/resolve-2.0.0-next.4.t(##################) ⠦ reify:@testing-library/react: http fetch GET 200 https://registry.npmjs.org/@testing-library/(##################) ⠇ reify:@typescript-eslint/utils: http fetch GET 200 https://registry.npmjs.org/@typescript-esl(##################) ⠋ reify:css-tree: http fetch GET 200 https://registry.npmjs.org/css-tree/-/css-tree-1.1.3.tgz 1(##################) ⠸ reify:css-tree: http fetch GET 200 https://registry.npmjs.org/css-tree/-/css-tree-1.1.3.tgz 1(##################) ⠧ reify:css-tree: http fetch GET 200 https://registry.npmjs.org/css-tree/-/css-tree-1.1.3.tgz 1(##################) ⠧ reify:css-tree: http fetch GET 200 https://registry.npmjs.org/css-tree/-/css-tree-1.1.3.tgz 1(##################) ⠴ reify:@babel/types: http fetch GET 200 https://registry.npmjs.org/@babel/types/-/types-7.21.3(##################) ⠴ reify:@babel/types: http fetch GET 200 https://registry.npmjs.org/@babel/types/-/types-7.21.3(##################) ⠴ reify:@babel/types: http fetch GET 200 https://registry.npmjs.org/@babel/types/-/types-7.21.3(##################) ⠴ reify:@babel/types: http fetch GET 200 https://registry.npmjs.org/@babel/types/-/types-7.21.3(##################) ⠴ reify:@babel/types: http fetch GET 200 https://registry.npmjs.org/@babel/types/-/types-7.21.3(##################) ⠴ reify:@babel/types: http fetch GET 200 https://registry.npmjs.org/@babel/types/-/types-7.21.3(##################) ⠴ reify:@babel/types: http fetch GET 200 https://registry.npmjs.org/@babel/types/-/types-7.21.3(##################) ⠧ reify:tailwindcss: http fetch GET 200 https://registry.npmjs.org/tailwindcss/-/tailwindcss-3.(##################) ⠧ reify:tailwindcss: http fetch GET 200 https://registry.npmjs.org/tailwindcss/-/tailwindcss-3.(##################) ⠏ reify:@typescript-eslint/scope-manager: http fetch GET 200 https://registry.npmjs.org/@typesc(##################) ⠏ reify:@typescript-eslint/scope-manager: http fetch GET 200 https://registry.npmjs.org/@typesc(##################) ⠙ reify:@typescript-eslint/scope-manager: http fetch GET 200 https://registry.npmjs.org/@typesc(##################) ⠧ reify:ajv: http fetch GET 200 https://registry.npmjs.org/ajv/-/ajv-8.12.0.tgz 15190ms (cache (##################) ⠴ reify:ajv: http fetch GET 200 https://registry.npmjs.org/ajv/-/ajv-8.12.0.tgz 14953ms (cache (##################) ⠏ reify:jsdom: http fetch GET 200 https://registry.npmjs.org/jsdom/-/jsdom-16.7.0.tgz 16510ms ((##################) ⠏ reify:jsdom: http fetch GET 200 https://registry.npmjs.org/jsdom/-/jsdom-16.7.0.tgz 16510ms ((##################) ⠏ reify:jsdom: http fetch GET 200 https://registry.npmjs.org/jsdom/-/jsdom-16.7.0.tgz 16510ms ((##################) ⠏ reify:jsdom: http fetch GET 200 https://registry.npmjs.org/jsdom/-/jsdom-16.7.0.tgz 16510ms ((##################) ⠏ reify:jsdom: http fetch GET 200 https://registry.npmjs.org/jsdom/-/jsdom-16.7.0.tgz 16510ms ((##################) ⠙ reify:caniuse-lite: http fetch GET 200 https://registry.npmjs.org/caniuse-lite/-/caniuse-lite(##################) ⠸ reify:webpack: http fetch GET 200 https://registry.npmjs.org/webpack/-/webpack-5.76.2.tgz 172(##################) ⠴ reify:lodash: http fetch GET 200 https://registry.npmjs.org/lodash/-/lodash-4.17.21.tgz 16873(##################) ⠴ reify:lodash: http fetch GET 200 https://registry.npmjs.org/lodash/-/lodash-4.17.21.tgz 16873(##################) ⠴ reify:lodash: http fetch GET 200 https://registry.npmjs.org/lodash/-/lodash-4.17.21.tgz 16873(##################) ⠴ reify:lodash: http fetch GET 200 https://registry.npmjs.org/lodash/-/lodash-4.17.21.tgz 16873(##################) ⠴ reify:lodash: http fetch GET 200 https://registry.npmjs.org/lodash/-/lodash-4.17.21.tgz 16873(##################) ⠴ reify:lodash: http fetch GET 200 https://registry.npmjs.org/lodash/-/lodash-4.17.21.tgz 16873(##################) ⠴ reify:lodash: http fetch GET 200 https://registry.npmjs.org/lodash/-/lodash-4.17.21.tgz 16873(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠧ reify:es-abstract: http fetch GET 200 https://registry.npmjs.org/es-abstract/-/es-abstract-1.(##################) ⠙ reify:core-js: http fetch GET 200 https://registry.npmjs.org/core-js/-/core-js-3.29.1.tgz 179(##################) ⠙ reify:core-js: http fetch GET 200 https://registry.npmjs.org/core-js/-/core-js-3.29.1.tgz 179(##################) ⠙ reify:core-js: http fetch GET 200 https://registry.npmjs.org/core-js/-/core-js-3.29.1.tgz 179(##################) ⠴ reify:typescript: http fetch GET 200 https://registry.npmjs.org/typescript/-/typescript-4.9.5(##################) ⠹ reify:typescript: http fetch GET 200 https://registry.npmjs.org/typescript/-/typescript-4.9.5(##################) ⠙ reify:typescript: http fetch GET 200 https://registry.npmjs.org/typescript/-/typescript-4.9.5(##################) ⠹ reify:typescript: http fetch GET 200 https://registry.npmjs.org/typescript/-/typescript-4.9.5

added 1488 packages, and audited 1489 packages in 22s

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


# =================
# DOCKER COMPOSE UP
# =================


 ✔ dynamodb-local 4 layers [⣿⣿⣿⣿]      0B/0B      Pulled                                                       10.8s 
   ✔ 1e78b99dd1fd Pull complete                                                                                 3.8s 
   ✔ 6aabd9041a5c Pull complete                                                                                 8.6s 
   ✔ 4f4fb700ef54 Pull complete                                                                                 8.6s 
   ✔ 601cf5909367 Pull complete                                                                                 9.7s 
 ✔ db 8 layers [⣿⣿⣿⣿⣿⣿⣿⣿]      0B/0B      Pulled                                                                9.9s 
   ✔ 63b65145d645 Pull complete                                                                                 1.2s 
   ✔ c441836541d9 Pull complete                                                                                 2.1s 
   ✔ d49de1a24361 Pull complete                                                                                 2.7s 
   ✔ 6c609d08dc3c Pull complete                                                                                 8.5s 
   ✔ e801cecfb07c Pull complete                                                                                 8.6s 
   ✔ 98756d431840 Pull complete                                                                                 8.7s 
   ✔ d991736c9c5a Pull complete                                                                                 8.7s 
   ✔ c708ebe2e647 Pull complete                                                                                 8.8s 
[+] Building 38.5s (18/18) FINISHED                                                                                  
 => [aws-bootcamp-cruddur-2023-backend-flask internal] load build definition from Dockerfile                    0.0s
 => => transferring dockerfile: 294B                                                                            0.0s
 => [aws-bootcamp-cruddur-2023-frontend-react-js internal] load build definition from Dockerfile                0.0s
 => => transferring dockerfile: 176B                                                                            0.0s
 => [aws-bootcamp-cruddur-2023-backend-flask internal] load .dockerignore                                       0.0s
 => => transferring context: 2B                                                                                 0.0s
 => [aws-bootcamp-cruddur-2023-frontend-react-js internal] load .dockerignore                                   0.0s
 => => transferring context: 2B                                                                                 0.0s
 => [aws-bootcamp-cruddur-2023-backend-flask internal] load metadata for docker.io/library/python:3.10-slim-bu  0.9s
 => [aws-bootcamp-cruddur-2023-frontend-react-js internal] load metadata for docker.io/library/node:16.18       0.8s
 => [aws-bootcamp-cruddur-2023-frontend-react-js 1/4] FROM docker.io/library/node:16.18@sha256:7f404d09ceb780  23.5s
 => => resolve docker.io/library/node:16.18@sha256:7f404d09ceb780c51f4fac7592c46b8f21211474aacce25389eb0df06aa  0.0s
 => => sha256:7f404d09ceb780c51f4fac7592c46b8f21211474aacce25389eb0df06aaa7472 776B / 776B                      0.0s
 => => sha256:620af4e91dbf80032eee9f1ff66a8b04119d7a329b2a13e007d69c8a0b337bf0 50.45MB / 50.45MB                0.7s
 => => sha256:fae29f309a72482bf13fbb1a8f4889ab9107fcad0c9fda76586aa55445e93ded 7.86MB / 7.86MB                  0.5s
 => => sha256:28fca74d99b6532401bfe63d36e1bafb1ac839564d48aa4e6e0a6aa2706a4d12 10.00MB / 10.00MB                0.5s
 => => sha256:46a10b2d8f2e9ae5c5e8ffedd5ae18a960d64b8c39c09e24fe2ee41d7148c249 2.21kB / 2.21kB                  0.0s
 => => sha256:993a4cf9c1e80aa74567d3deea4dfa1488b94dcb024bfca9246f979845763509 7.51kB / 7.51kB                  0.0s
 => => sha256:0b5db87f5b42af9f258f14f367616814cb9b518ea0141f46bdd2706bb256d408 51.84MB / 51.84MB                1.5s
 => => sha256:fa488706ea13a788b351252b655f6ccb88201c4bace57cf25408fda65758c518 191.89MB / 191.89MB              3.7s
 => => sha256:0380b9b3282fe25f00e7d8191dacb0167d90b7b881f05ff9b1ca72bcd38b9a6b 4.20kB / 4.20kB                  0.8s
 => => extracting sha256:620af4e91dbf80032eee9f1ff66a8b04119d7a329b2a13e007d69c8a0b337bf0                       5.9s
 => => sha256:383dfecd36873ac6c0fc1feb73b2febfa30a5502bea0566c51cf170234248004 34.97MB / 34.97MB                1.7s
 => => sha256:ca59981dc274124ea3f9d421b039e54062b53aba0c04f536bbe2545a80bdba51 2.28MB / 2.28MB                  1.9s
 => => sha256:4fa5c4b55a850ac871248b30c51c35c6c77adbc12258b823a725d84a6853dbc2 450B / 450B                      1.8s
 => => extracting sha256:fae29f309a72482bf13fbb1a8f4889ab9107fcad0c9fda76586aa55445e93ded                       0.7s
 => => extracting sha256:28fca74d99b6532401bfe63d36e1bafb1ac839564d48aa4e6e0a6aa2706a4d12                       0.7s
 => => extracting sha256:0b5db87f5b42af9f258f14f367616814cb9b518ea0141f46bdd2706bb256d408                       2.4s
 => => extracting sha256:fa488706ea13a788b351252b655f6ccb88201c4bace57cf25408fda65758c518                       7.7s
 => => extracting sha256:0380b9b3282fe25f00e7d8191dacb0167d90b7b881f05ff9b1ca72bcd38b9a6b                       0.0s
 => => extracting sha256:383dfecd36873ac6c0fc1feb73b2febfa30a5502bea0566c51cf170234248004                       1.5s
 => => extracting sha256:ca59981dc274124ea3f9d421b039e54062b53aba0c04f536bbe2545a80bdba51                       0.1s
 => => extracting sha256:4fa5c4b55a850ac871248b30c51c35c6c77adbc12258b823a725d84a6853dbc2                       0.0s
 => [aws-bootcamp-cruddur-2023-frontend-react-js internal] load build context                                  10.0s
 => => transferring context: 241.43MB                                                                           9.6s
 => [aws-bootcamp-cruddur-2023-backend-flask 1/5] FROM docker.io/library/python:3.10-slim-buster@sha256:6ba3f  10.5s
 => => resolve docker.io/library/python:3.10-slim-buster@sha256:6ba3f89c82d17db0a71fc56d553e5d251e3a248e8722c3  0.0s
 => => sha256:6ba3f89c82d17db0a71fc56d553e5d251e3a248e8722c3977525819ddf4c957e 988B / 988B                      0.0s
 => => sha256:31827b60ef2becea7b6b017f309c57062f7b3f37ad309eb57e9ed20411690c01 1.37kB / 1.37kB                  0.0s
 => => sha256:a8bd408e774ad6e6b3d4dbb2d2fd00f46202e835674c34da1f1f3f1b2879ad7e 6.90kB / 6.90kB                  0.0s
 => => sha256:3689b8de819b48387712c6d4d62d26a52a04c9e88afc68fb9d1dbe48bfa9e21d 27.14MB / 27.14MB                2.3s
 => => sha256:af8cd5f36469921b82be5c046d0fe82365de8fcee96a4caa8259939d06d99bef 2.78MB / 2.78MB                  2.2s
 => => sha256:c320fc4822af2adac19430752a39ed8efccbf30c52a57b244ef013fea1931df7 11.51MB / 11.51MB                2.4s
 => => sha256:d4b0a1dbff806bc633e2572a00b68c67e0c346399273f51dbe7c93cfd715d9ab 245B / 245B                      2.5s
 => => sha256:d53646ea279baf0fc070eed82bc8743b094a47492ad53ad70c786cb690605f56 3.37MB / 3.37MB                  2.6s
 => => extracting sha256:3689b8de819b48387712c6d4d62d26a52a04c9e88afc68fb9d1dbe48bfa9e21d                       3.7s
 => => extracting sha256:af8cd5f36469921b82be5c046d0fe82365de8fcee96a4caa8259939d06d99bef                       0.5s
 => => extracting sha256:c320fc4822af2adac19430752a39ed8efccbf30c52a57b244ef013fea1931df7                       1.2s
 => => extracting sha256:d4b0a1dbff806bc633e2572a00b68c67e0c346399273f51dbe7c93cfd715d9ab                       0.0s
 => => extracting sha256:d53646ea279baf0fc070eed82bc8743b094a47492ad53ad70c786cb690605f56                       0.3s
 => [aws-bootcamp-cruddur-2023-backend-flask internal] load build context                                       0.0s
 => => transferring context: 20.91kB                                                                            0.0s
 => [aws-bootcamp-cruddur-2023-backend-flask 2/5] WORKDIR /backend-flask                                        0.0s
 => [aws-bootcamp-cruddur-2023-backend-flask 3/5] COPY requirements.txt requirements.txt                        0.0s
 => [aws-bootcamp-cruddur-2023-backend-flask 4/5] RUN pip3 install -r requirements.txt                          7.5s
 => [aws-bootcamp-cruddur-2023-backend-flask 5/5] COPY . .                                                      0.3s
 => [aws-bootcamp-cruddur-2023-frontend-react-js] exporting to image                                            7.5s
 => => exporting layers                                                                                         6.7s
 => => writing image sha256:df0b787985d1bbb17dc6eaf9b5c390690f585e95953497c365f408c1be558432                    0.0s
 => => naming to docker.io/library/aws-bootcamp-cruddur-2023-backend-flask                                      0.0s
 => => writing image sha256:46bc2e99734b47d0bf71ed3bb9489c51d1f12887e0713282007fa7b279af206c                    0.0s
 => => naming to docker.io/library/aws-bootcamp-cruddur-2023-frontend-react-js                                  0.0s
 => [aws-bootcamp-cruddur-2023-frontend-react-js 2/4] COPY . /frontend-react-js                                 4.1s
 => [aws-bootcamp-cruddur-2023-frontend-react-js 3/4] WORKDIR /frontend-react-js                                0.0s
 => [aws-bootcamp-cruddur-2023-frontend-react-js 4/4] RUN npm install                                           3.3s
[+] Running 6/2
 ✔ Network aws-bootcamp-cruddur-2023_default                Crea...                                             0.0s 
 ✔ Volume "aws-bootcamp-cruddur-2023_db"                    Created                                             0.0s 
 ✔ Container aws-bootcamp-cruddur-2023-db-1                 Creat...                                            0.0s 
 ✔ Container aws-bootcamp-cruddur-2023-frontend-react-js-1  Created                                             0.0s 
 ✔ Container aws-bootcamp-cruddur-2023-backend-flask-1      Created                                             0.0s 
 ✔ Container dynamodb-local                                 Created                                             0.0s 
Attaching to aws-bootcamp-cruddur-2023-backend-flask-1, aws-bootcamp-cruddur-2023-db-1, aws-bootcamp-cruddur-2023-frontend-react-js-1, dynamodb-local
dynamodb-local                                 | Initializing DynamoDB Local with the following configuration:
dynamodb-local                                 | Port:  8000
dynamodb-local                                 | InMemory:      false
dynamodb-local                                 | DbPath:        ./data
dynamodb-local                                 | SharedDb:      true
dynamodb-local                                 | shouldDelayTransientStatuses:  false
dynamodb-local                                 | CorsParams:    null
dynamodb-local                                 | 
aws-bootcamp-cruddur-2023-db-1                 | The files belonging to this database system will be owned by user "postgres".
aws-bootcamp-cruddur-2023-db-1                 | This user must also own the server process.
aws-bootcamp-cruddur-2023-db-1                 | 
aws-bootcamp-cruddur-2023-db-1                 | The database cluster will be initialized with locale "en_US.utf8".
aws-bootcamp-cruddur-2023-db-1                 | The default database encoding has accordingly been set to "UTF8".
aws-bootcamp-cruddur-2023-db-1                 | The default text search configuration will be set to "english".
aws-bootcamp-cruddur-2023-db-1                 | 
aws-bootcamp-cruddur-2023-db-1                 | Data page checksums are disabled.
aws-bootcamp-cruddur-2023-db-1                 | 
aws-bootcamp-cruddur-2023-db-1                 | fixing permissions on existing directory /var/lib/postgresql/data ... ok
aws-bootcamp-cruddur-2023-db-1                 | creating subdirectories ... ok
aws-bootcamp-cruddur-2023-db-1                 | selecting dynamic shared memory implementation ... posix
aws-bootcamp-cruddur-2023-db-1                 | selecting default max_connections ... 100
aws-bootcamp-cruddur-2023-db-1                 | selecting default shared_buffers ... 128MB
aws-bootcamp-cruddur-2023-db-1                 | selecting default time zone ... UTC
aws-bootcamp-cruddur-2023-db-1                 | creating configuration files ... ok
aws-bootcamp-cruddur-2023-db-1                 | running bootstrap script ... ok
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-frontend-react-js-1  | > frontend@0.1.0 start
aws-bootcamp-cruddur-2023-frontend-react-js-1  | > react-scripts start
aws-bootcamp-cruddur-2023-frontend-react-js-1  | 
aws-bootcamp-cruddur-2023-db-1                 | sh: locale: not found
aws-bootcamp-cruddur-2023-db-1                 | 2023-03-25 00:59:25.951 UTC [48] WARNING:  no usable system locales were found
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
aws-bootcamp-cruddur-2023-db-1                 | performing post-bootstrap initialization ... ok
aws-bootcamp-cruddur-2023-backend-flask-1      | 'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
aws-bootcamp-cruddur-2023-backend-flask-1      | 'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
aws-bootcamp-cruddur-2023-backend-flask-1      | 'FLASK_ENV' is deprecated and will not be used in Flask 2.3. Use 'FLASK_DEBUG' instead.
aws-bootcamp-cruddur-2023-backend-flask-1      |  * Debugger is active!
aws-bootcamp-cruddur-2023-backend-flask-1      |  * Debugger PIN: 322-166-266
aws-bootcamp-cruddur-2023-db-1                 | syncing data to disk ... ok
aws-bootcamp-cruddur-2023-db-1                 | 
aws-bootcamp-cruddur-2023-db-1                 | 
aws-bootcamp-cruddur-2023-db-1                 | Success. You can now start the database server using:
aws-bootcamp-cruddur-2023-db-1                 | 
aws-bootcamp-cruddur-2023-db-1                 |     pg_ctl -D /var/lib/postgresql/data -l logfile start
aws-bootcamp-cruddur-2023-db-1                 | 
aws-bootcamp-cruddur-2023-db-1                 | initdb: warning: enabling "trust" authentication for local connections
aws-bootcamp-cruddur-2023-db-1                 | You can change this by editing pg_hba.conf or using the option -A, or
aws-bootcamp-cruddur-2023-db-1                 | --auth-local and --auth-host, the next time you run initdb.
aws-bootcamp-cruddur-2023-db-1                 | waiting for server to start....2023-03-25 00:59:26.750 UTC [54] LOG:  starting PostgreSQL 13.10 on x86_64-pc-linux-musl, compiled by gcc (Alpine 12.2.1_git20220924-r4) 12.2.1 20220924, 64-bit
aws-bootcamp-cruddur-2023-db-1                 | 2023-03-25 00:59:26.751 UTC [54] LOG:  listening on Unix socket "/var/run/postgresql/.s.PGSQL.5432"
aws-bootcamp-cruddur-2023-db-1                 | 2023-03-25 00:59:26.754 UTC [55] LOG:  database system was shut down at 2023-03-25 00:59:26 UTC
aws-bootcamp-cruddur-2023-db-1                 | 2023-03-25 00:59:26.756 UTC [54] LOG:  database system is ready to accept connections
aws-bootcamp-cruddur-2023-db-1                 |  done
aws-bootcamp-cruddur-2023-db-1                 | server started
aws-bootcamp-cruddur-2023-db-1                 | 
aws-bootcamp-cruddur-2023-db-1                 | /usr/local/bin/docker-entrypoint.sh: ignoring /docker-entrypoint-initdb.d/*
aws-bootcamp-cruddur-2023-db-1                 | 
aws-bootcamp-cruddur-2023-db-1                 | waiting for server to shut down....2023-03-25 00:59:26.851 UTC [54] LOG:  received fast shutdown request
aws-bootcamp-cruddur-2023-db-1                 | 2023-03-25 00:59:26.852 UTC [54] LOG:  aborting any active transactions
aws-bootcamp-cruddur-2023-db-1                 | 2023-03-25 00:59:26.853 UTC [54] LOG:  background worker "logical replication launcher" (PID 61) exited with exit code 1
aws-bootcamp-cruddur-2023-db-1                 | 2023-03-25 00:59:26.853 UTC [56] LOG:  shutting down
aws-bootcamp-cruddur-2023-db-1                 | 2023-03-25 00:59:26.862 UTC [54] LOG:  database system is shut down
aws-bootcamp-cruddur-2023-db-1                 |  done
aws-bootcamp-cruddur-2023-db-1                 | server stopped
aws-bootcamp-cruddur-2023-db-1                 | 
aws-bootcamp-cruddur-2023-db-1                 | PostgreSQL init process complete; ready for start up.
aws-bootcamp-cruddur-2023-db-1                 | 
aws-bootcamp-cruddur-2023-db-1                 | 2023-03-25 00:59:26.968 UTC [1] LOG:  starting PostgreSQL 13.10 on x86_64-pc-linux-musl, compiled by gcc (Alpine 12.2.1_git20220924-r4) 12.2.1 20220924, 64-bit
aws-bootcamp-cruddur-2023-db-1                 | 2023-03-25 00:59:26.968 UTC [1] LOG:  listening on IPv4 address "0.0.0.0", port 5432
aws-bootcamp-cruddur-2023-db-1                 | 2023-03-25 00:59:26.968 UTC [1] LOG:  listening on IPv6 address "::", port 5432
aws-bootcamp-cruddur-2023-db-1                 | 2023-03-25 00:59:26.970 UTC [1] LOG:  listening on Unix socket "/var/run/postgresql/.s.PGSQL.5432"
aws-bootcamp-cruddur-2023-db-1                 | 2023-03-25 00:59:26.972 UTC [67] LOG:  database system was shut down at 2023-03-25 00:59:26 UTC
aws-bootcamp-cruddur-2023-db-1                 | 2023-03-25 00:59:26.975 UTC [1] LOG:  database system is ready to accept connections
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
