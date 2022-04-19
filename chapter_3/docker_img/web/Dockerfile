# 1. node 설치 (FROM : 베이스 이미지 지정)
FROM node:12-alpine 

COPY ./package* /usr/src/app/ 
WORKDIR /usr/src/app 
RUN npm install 
# RUN : 명령어 실행

# 2. 소스 복사 (COPY : 로컬 파일을 이미지로 복사)
COPY . /usr/src/app

# 3. Nodejs 패키지 설치 (WORKDIR : 이동할 디렉토리 지정)
WORKDIR /usr/src/app 

# 4. WEB 서버 실행 (Listen 포트 정의) (EXPOSE : 포트정보 전달, CMD : 컨테이너 생성 시 실행할 명령어)
EXPOSE 3000 
CMD node app.js