# Week 0 — Billing and Architecture

# ========================
# GITPOD WORKSPACE STARTUP
# ========================

HISTFILE=/workspace/.gitpod/cmd-1 history -r; {
curl -fsSL https://www.postgresql.org/media/keys/ACCC4CF8.asc|sudo gpg --dearmor -o /etc/apt/trusted.gpg.d/postgresql.gpg
echo "deb http://apt.postgresql.org/pub/repos/apt/ `lsb_release -cs`-pgdg main" |sudo tee  /etc/apt/sources.list.d/pgdg.list
sudo apt update
sudo apt install -y postgresql-client-13 libpq-dev

}
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $  HISTFILE=/workspace/.gitpod/cmd-1 history -r; {
> curl -fsSL https://www.postgresql.org/media/keys/ACCC4CF8.asc|sudo gpg --dearmor -o /etc/apt/trusted.gpg.d/postgresql.gpg
> echo "deb http://apt.postgresql.org/pub/repos/apt/ `lsb_release -cs`-pgdg main" |sudo tee  /etc/apt/sources.list.d/pgdg.list
> sudo apt update
> sudo apt install -y postgresql-client-13 libpq-dev
> 
> }
deb http://apt.postgresql.org/pub/repos/apt/ focal-pgdg main
Get:1 https://download.docker.com/linux/ubuntu focal InRelease [57.7 kB]
Hit:2 http://archive.ubuntu.com/ubuntu focal InRelease                         
Get:3 http://security.ubuntu.com/ubuntu focal-security InRelease [114 kB]      
Get:4 http://archive.ubuntu.com/ubuntu focal-updates InRelease [114 kB]        
Get:5 https://download.docker.com/linux/ubuntu focal/stable amd64 Packages [28.7 kB]
Get:6 http://ppa.launchpad.net/git-core/ppa/ubuntu focal InRelease [23.8 kB]   
Get:8 http://apt.postgresql.org/pub/repos/apt focal-pgdg InRelease [91.6 kB]   
Get:9 http://archive.ubuntu.com/ubuntu focal-backports InRelease [108 kB]      
Get:7 https://apt.llvm.org/focal llvm-toolchain-focal-15 InRelease [6,833 B]   
Get:10 http://security.ubuntu.com/ubuntu focal-security/multiverse amd64 Packages [28.5 kB]
Get:11 http://security.ubuntu.com/ubuntu focal-security/universe amd64 Packages [1,019 kB]
Get:12 http://archive.ubuntu.com/ubuntu focal-updates/universe amd64 Packages [1,314 kB]
Get:13 http://ppa.launchpad.net/ondrej/apache2/ubuntu focal InRelease [23.8 kB]
Get:14 https://apt.llvm.org/focal llvm-toolchain-focal-15/main amd64 Packages [12.4 kB]
Get:15 http://security.ubuntu.com/ubuntu focal-security/restricted amd64 Packages [2,003 kB]
Get:16 http://archive.ubuntu.com/ubuntu focal-updates/multiverse amd64 Packages [31.2 kB]
Get:17 http://archive.ubuntu.com/ubuntu focal-updates/restricted amd64 Packages [2,141 kB]
Get:18 http://security.ubuntu.com/ubuntu focal-security/main amd64 Packages [2,549 kB]
Get:19 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 Packages [3,027 kB]
Get:20 http://ppa.launchpad.net/ondrej/nginx-mainline/ubuntu focal InRelease [23.8 kB]
Get:21 http://apt.postgresql.org/pub/repos/apt focal-pgdg/main amd64 Packages [419 kB]
Get:22 http://archive.ubuntu.com/ubuntu focal-backports/main amd64 Packages [55.2 kB]
Get:23 http://archive.ubuntu.com/ubuntu focal-backports/universe amd64 Packages [28.6 kB]
Get:24 http://ppa.launchpad.net/ondrej/php/ubuntu focal InRelease [23.9 kB]    
Get:25 http://ppa.launchpad.net/git-core/ppa/ubuntu focal/main amd64 Packages [3,160 B]
Get:26 http://ppa.launchpad.net/ondrej/apache2/ubuntu focal/main amd64 Packages [4,907 B]
Get:27 http://ppa.launchpad.net/ondrej/nginx-mainline/ubuntu focal/main amd64 Packages [6,422 B]
Get:28 http://ppa.launchpad.net/ondrej/php/ubuntu focal/main amd64 Packages [194 kB]
Fetched 13.5 MB in 3s (4,044 kB/s)                    
Reading package lists... Done
Building dependency tree       
Reading state information... Done
138 packages can be upgraded. Run 'apt list --upgradable' to see them.
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following additional packages will be installed:
  libpq5 postgresql-client-common
Suggested packages:
  postgresql-doc-15 postgresql-13 postgresql-doc-13
The following NEW packages will be installed:
  postgresql-client-13 postgresql-client-common
The following packages will be upgraded:
  libpq-dev libpq5
2 upgraded, 2 newly installed, 0 to remove and 136 not upgraded.
Need to get 1,923 kB of archives.
After this operation, 7,315 kB of additional disk space will be used.
Get:1 http://apt.postgresql.org/pub/repos/apt focal-pgdg/main amd64 libpq-dev amd64 15.2-1.pgdg20.04+1 [140 kB]
Get:2 http://apt.postgresql.org/pub/repos/apt focal-pgdg/main amd64 libpq5 amd64 15.2-1.pgdg20.04+1 [183 kB]
Get:3 http://apt.postgresql.org/pub/repos/apt focal-pgdg/main amd64 postgresql-client-common all 248.pgdg20.04+1 [92.7 kB]
Get:4 http://apt.postgresql.org/pub/repos/apt focal-pgdg/main amd64 postgresql-client-13 amd64 13.10-1.pgdg20.04+1 [1,507 kB]
Fetched 1,923 kB in 1s (1,430 kB/s)             
debconf: delaying package configuration, since apt-utils is not installed
(Reading database ... 36107 files and directories currently installed.)
Preparing to unpack .../libpq-dev_15.2-1.pgdg20.04+1_amd64.deb ...
Unpacking libpq-dev (15.2-1.pgdg20.04+1) over (12.12-0ubuntu0.20.04.1) ...
Preparing to unpack .../libpq5_15.2-1.pgdg20.04+1_amd64.deb ...
Unpacking libpq5:amd64 (15.2-1.pgdg20.04+1) over (12.12-0ubuntu0.20.04.1) ...
Selecting previously unselected package postgresql-client-common.
Preparing to unpack .../postgresql-client-common_248.pgdg20.04+1_all.deb ...
Unpacking postgresql-client-common (248.pgdg20.04+1) ...
Selecting previously unselected package postgresql-client-13.
Preparing to unpack .../postgresql-client-13_13.10-1.pgdg20.04+1_amd64.deb ...
Unpacking postgresql-client-13 (13.10-1.pgdg20.04+1) ...
Setting up postgresql-client-common (248.pgdg20.04+1) ...
Setting up libpq5:amd64 (15.2-1.pgdg20.04+1) ...
Setting up libpq-dev (15.2-1.pgdg20.04+1) ...
Setting up postgresql-client-13 (13.10-1.pgdg20.04+1) ...
update-alternatives: using /usr/share/postgresql/13/man/man1/psql.1.gz to provide /usr/share/man/man1/psql.1.gz (psql.1.gz) in auto mode
Processing triggers for man-db (2.9.1-1) ...
Processing triggers for libc-bin (2.31-0ubuntu9.9) ...
gitpod /workspace/aws-bootcamp-cruddur-2023 (main) $ 

