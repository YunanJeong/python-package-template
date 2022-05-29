# python_package_test
practice. how to make python package

## 파일 및 디렉토리 설명
    package/
        __init__.py             # 해당 디렉토리가 패키지임을 명시
        __main__.py             # 메인 실행시 시작 파일
        util.py                 # 로직 모음
        version.py              # 버전 표기

    setup.py                    # 설치


## 설치
- 레포지토리 최상위 경로에서 다음 커맨드 실행
    - `pip install -e . `


## 실행
- `python -m packagename [-h] -r REQUIRED [-s START] [-e END]`
- 예시 :
    - `python -m packagename -r "required"`
    - `python -m packagename -r "required" -s "start" -e "end"`


## 필요 모듈
- 파이썬 패키지
    - `pip install -r requirements.txt`
    - (awscli1 필요, requirements.txt에는 미포함)


## 기타 메모
- 설치방법 관련: 이는 PyPI 에 배포하기 위한 방법이 아니라, 소스코드 전체를 git 등으로 공유할 떄 사용할 수 있는 방법임.
- -e 옵션은 editable을 의미. 패키지 설치해도 파이썬 패키지지정경로에서 소스코드가 있는 경로를 참조하기 떄문에 재설치없이 계속 편집가능.