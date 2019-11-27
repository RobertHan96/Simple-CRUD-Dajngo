# Simple-CRUD-Dajngo

장고 개발 정리 

#장고 manage.py 주요 명령어 
- Makemigrations :  db에 새로운 변동사항이 있는지 체크 
- Migrate : db의 변동사항을 서버에 반영
- Run server : 서버실행  뒤에 서버실행할 로컬주소 설정 가능 => 0.0.0.0:8000


1) 프로젝트 초기 설정
1. 파이참으로 장고 프로젝트 실행 
2. startapp {앱이름} 
3. {앱이름} -> apps.py 에서 Config 클래스 이름 복사 
4. 프로젝트 디렉토리 -> settings.py -> INSTALLED_APPS 안에 이름 붙여 넣기 
5. settings.py에서 TIME_ZONE을 서울로 변경
6. models.py에서 db테이블 생성 
7. admin.py에 db내용 반영 : from {앱이름}.models import {models.py에서 생성한 클래스명} 
8. admin.py에서 생성한 디비를 추척할 수 있도록 코드 추가 :  admin.site.register(models.py에서 생성한 클래스명)
9.  manage.py에서 DB 마이그레이션 명령어 진행 
		ㄴ makemigrations => migrate 
10.  어드민 계정 생성 : manage.py => createsuperuser 
11. Runserver 명령어 실행하여 제대로 반영되었는지 확인
    1. 메인화면에서 장고 로켓 모양 출력 
    2. /admin 주소에서 로그인 후 앞서 만든 db 테이블 구조 생성되었는지 확인
12. 
