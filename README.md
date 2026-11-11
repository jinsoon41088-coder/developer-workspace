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
### Windows 운영체제 버전 확인
### PowerShell 버전 확인
### Git 버전 확인
### Docker 버전 확인
### Ubuntu 버전 확인

실행 명령어:

```powershell
wsl -d Ubuntu -- cat /etc/os-release
```

실행 결과:

```text
VERSION="26.04.1 LTS (Resolute Raccoon)"
VERSION_CODENAME=resolute
ID=ubuntu
ID_LIKE=debian
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
UBUNTU_CODENAME=resolute
LOGO=ubuntu-logo
```

확인된 Ubuntu 버전: 26.04.1 LTS (Resolute Raccoon)
실행 명령어:

```powershell
docker --version
```

실행 결과:

```text
Docker version 29.9.2, build a82e528
```

확인된 Docker 버전: 29.9.2
실행 명령어:

```powershell
git --version
```

실행 결과:

```text
git version 2.56.0.windows.4
```

확인된 Git 버전: 2.56.0.windows.4
실행 명령어:

```powershell
$PSVersionTable.PSVersion
```

실행 결과:

```text
Major  Minor  Build  Revision
-----  -----  -----  --------
5      1      26100  9711
```

확인된 버전: Windows PowerShell 5.1.26100.9711
실행 명령어:

```powershell
Get-ComputerInfo | Select-Object WindowsProductName, OsVersion, OsBuildNumber
```

실행 결과:

```text
WindowsProductName OsVersion  OsBuildNumber
------------------ ---------  -------------
Windows 10 Pro     10.0.26300 26300
```

참고: WindowsProductName은 Windows 10 Pro로 표시되지만, 빌드 26300은 Windows 11 계열입니다.
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
## 6. GitHub 저장소

- 저장소 이름: developer-workspace
- GitHub 계정: jinsoon41088-coder
- 저장소 주소: https://github.com/jinsoon41088-coder/developer-workspace
- 기본 브랜치: main
- GitHub 업로드: 완료