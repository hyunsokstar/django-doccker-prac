From ubuntu:18.04

RUN apt-get update && apt-get install -y python3-pip python3-dev && apt-get clean

WORKDIR /code/
# ADD ./backend ./code
ADD ./backend ./code
RUN pip3 install -r requirements.txt

EXPOSE 8000
CMD ["python3", "manage.py", "runserver", "0.0.0.0:8000"]

# www.inflearn.com/course/파이썬-장고-웹서비스/unit/90661?tab=community&q=784499&category=questionDetail
# docker build -t test_dj .
# docker run --rm test_dj

# Mac:

# 오른쪽 상단의 검색> Keychain 입력> Keychain Access> github 관련 password 삭제

# Windows:

# 제어판> 제어판 검색> 자격 입력> 자격 증명 관리자> github 관련 password 삭제

# 후 다시 하면 문제가 없다.
