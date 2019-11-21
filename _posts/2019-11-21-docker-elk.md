[참고] docker, docker-compose

https://www.44bits.io/ko/post/almost-perfect-development-environment-with-docker-and-docker-compose#%EC%82%AC%EC%A0%84-%ED%95%99%EC%8A%B5-%EB%8F%84%EC%BB%A4%EA%B0%80-%EB%AD%90%EC%95%BC

설치 및 설정
1. EC2 인스턴스에 docker 및 docker-compose 설치

#Docker 설치

$ sudo yum -y install docker

$ sudo chkconfig –add docker

$ sudo -i service docker start

$ sudo usermod -aG docker ec2-user

#Docker-compose 설치

$ sudo curl -L “https://github.com/docker/compose/releases/download/1.24.1/docker-compose-$(uname -s)-$(uname -m)” -o /usr/local/bin/docker-compose

$ sudo chmod +x /usr/local/bin/docker-compose


2. docker-compose 구성

-


3. logstash/pipeline/logstash.conf 수정
<script src="https://gist.github.com/leeilly/37121a58798b882d6987b1a43b7730ec.js"></script>
