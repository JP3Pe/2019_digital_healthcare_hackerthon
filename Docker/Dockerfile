# 1. 데비안을 업데이트
FROM Debian
MAINTAINER jkkim.work@gmail.com
RUN apt update && apt full-upgrade -y

# 2. Python3, pip, git 설치
RUN apt install python3 python3-pip git -y

# 3. pip3 이용해 elasticbeanstalk(awsebcli) 설치, 설치된 패키지 환경 변수에 등록
RUN pip3 install awsebcli --upgrade --userupgrade --user && PATH=$PATH:/root/.local/bin