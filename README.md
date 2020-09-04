# GitLab Server 설치 과정

1. Install and configure the necessary dependencies
<br>1.1 `sudo apt-get update`
<br>1.2 `sudo apt-get install -y curl openssh-server ca-certificates tzdata`
<br>1.3 `sudo apt-get install -y postfix`

2. Add the GitLab package repository and install package
<br> 2-1. `curl https://packages.gitlab.com/install/repositories/gitlab/gitlab-ee/script.deb.sh | sudo bash`
<br> 2-2. `sudo EXTERNAL_URL="https://gitlab.example.com" apt-get install gitlab-ee`

3.  Browse to the hostname and login

* 서버 실행 : `sudo gitlab-ctl start`
* 서버 중단 : `sudo gitlab-ctl stop`
* 서버 재시작 : `suto gitlab-ctl restart`
* **root 계정 아이디 : root / 비밀번호 : espresomedia!**

    [**Gitlab 사이트**](https://about.gitlab.com/)
    <br>
    [**Gitlab 다운로드 사이트**](https://about.gitlab.com/install/)
    <br>
    [**Gitlab Private Repository User Permission**](https://www.tutorialspoint.com/gitlab/gitlab_user_permissions.htm)
    <br>
    [**치타 Gitlab Site**](http:172.30.1.58)
