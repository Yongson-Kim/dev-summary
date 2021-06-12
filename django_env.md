# Django 개발환경 설정

## 가상환경 생성

```bash
$ mkdir project_root_name
$ cd project_root_name
project_root_name $ python3 -m venv venv_name
project_root_name $ source ./venv_name/bin/activate
(venv_name) project_root_name $
```

## Django 설치

**가상환경**에서 실행합니다.

```bash
(venv_name) project_root_name $ pip install django
```


가상환경에서 종속성 목록 생성
프로젝트 루트 디렉토리에서 실행
```bash
pip freeze > requirements.txt
```


가상환경에서 종속성 패키지 복원
```bash
python -m pip install -r requirements.txt
```