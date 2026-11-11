# 개발자용 작업실 꾸미기

## 1. 프로젝트 소개
Windows 11, Ubuntu, Docker, Git을 활용하여
개발 환경을 구성하고 기본 명령어를 실습한 프로젝트입니다.

## 2. 실행 환경
- OS: Windows 11
- Linux: Ubuntu (WSL2)
- Terminal: PowerShell, Ubuntu Bash
- Docker: Docker Desktop
- Git: Git

## 3. 수행 항목
- [x] PowerShell 기본 명령어
- [x] Ubuntu CLI 명령어
- [x] 파일 권한 변경
- [x] Bash 스크립트 실행
- [x] Docker 컨테이너 실행
- [x] Dockerfile 이미지 빌드
- [x] Docker 포트 매핑
- [x] Docker 바인드 마운트
- [x] Docker 볼륨
- [x] Git 저장소 초기화
- [ ] Git 커밋 및 GitHub 업로드

## 4. Docker 실행 검증

### hello-world
```bash
docker run hello-world
```
결과: Hello from Docker!

### Docker 이미지 빌드
```bash
docker build -t pink-panda:1.0 .
docker run --rm pink-panda:1.0
```
결과: Hello Pink Panda Docker!

### 포트 매핑
```bash
docker run -d --name panda-web -p 8080:80 nginx:alpine
```
결과: http://localhost:8080 에서 Nginx 페이지 확인

### 바인드 마운트
결과: http://localhost:8081 에서 핑크판다 웹사이트 확인

### Docker 볼륨
```bash
docker volume create panda-data
docker volume ls
```
결과: Hello Pink Panda Volume!

## 5. 추가 기록 예정
- 실행 도구의 정확한 버전
- 터미널 명령어와 출력 로그
- 파일 권한 검증
- Git 커밋 기록
- GitHub 저장소 링크
- 수행 증거 스크린샷
