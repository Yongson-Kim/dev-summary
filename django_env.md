# Django 개발환경 설정

## Project Root 폴더 생성

```bash
$ mkdir project_root_name
$ cd project_root_name
```

## 가상환경 생성

* 가상환경명: `venv`

```bash
project_root_name $ python3 -m venv devenv
project_root_name $ source ./venv_name/bin/activate
(venv) project_root_name $
```

## Django 및 관련 모듈 설치

**가상환경(venv)**에서 실행

```bash
(venv) project_root_name $ pip install django
(venv) project_root_name $ pip install django-environ
(venv) project_root_name $ pip install django-bootstrap4
```

가상환경에서 사용한 종속성 목록 생성
프로젝트 루트 디렉토리에서 실행

```bash
(venv) project_root_name $ pip freeze > requirements.txt
```

## 기존 소스를 새로받을 경우

* **가상환경**에서 종속성 패키지 복원
* Model 생성 (sqlite)

```bash
(venv) project_root_name $ pip install -r requirements.txt
(venv) project_root_name $ python3 manage.py makemigrations
(venv) project_root_name $ python3 manage.py migrate
```


## Server 실행



## Debugging




## Nginx - Gunicorn - Django

Docker Volume
- Bind Volume
- Named Volume