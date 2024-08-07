# sudo docker exec -it gitlab /bin/bash
# cat /etc/gitlab/initial_root_password


# external_url 안된다면 cat /etc/gitlab/gitlab.rb > 아래 ssl 관련 내용 추가
# $ sudo gitlab-ctl reconfigure	#설정파일 반영
# 참고
# $ sudo gitlab-ctl start   #gitlab 실행
# $ sudo gitalb-ctl stop    #gitlab 중지
# $ sudo gitlab-ctl restart #gitlab 재실행
# sudo docker exec -it gitlab-be /bin/bash

# 포트 출돌 관련
https://codingdog.tistory.com/entry/gitlab-8080-%ED%8F%AC%ED%8A%B8-%EB%8C%80%EC%8B%A0-%EB%8B%A4%EB%A5%B8-%ED%8F%AC%ED%8A%B8%EB%A5%BC-%EC%82%AC%EC%9A%A9%ED%95%98%EA%B2%8C-%EB%B0%94%EA%BF%94%EB%B4%85%EC%8B%9C%EB%8B%A4


# 로컬 url 셋팅
Windows
메모장을 관리자 권한으로 엽니다.

C:\Windows\System32\drivers\etc\hosts 파일을 엽니다.

다음 줄을 추가합니다:

```
127.0.0.1 gitlab.local
127.0.0.1 backend.local
```

MacOS / Linux
터미널을 엽니다.

sudo nano /etc/hosts 명령어를 사용하여 hosts 파일을 엽니다.

다음 줄을 추가합니다:
```
127.0.0.1 gitlab.local
127.0.0.1 backend.local
```