# Mac os brew를 이용해 mysql 설치

`brew search mysql`

- mysql에 관련된 프로그램들을 검색

`brew install mysql`

- 설치하기

`brew services start mysql`

- mysql서비스를 우선 켜줌.

`mysql -uroot`

- 기본계정인 root로 로그인하기.
- 디폴트로 비밀번호가 설정되어 있지 않아 비밀번호를 설정하려면
  - ` mysql_secure_installation`

mysql> 이 출력되면 mysql이 성공적으로 실행된 것임.

---

## 내가 겪은 에러

```
 ERROR! The server quit without updating PID file (/opt/homebrew/var/mysql/amoo-Arirangui-MacBookPro.local.pid).
```

이는 여러번의 mysql재설치를 통해 해결했는데 계속 같은 문제가 발생했음.

- brew로 설치한 패키지 중 brew upgrade이후 최신 버전이 아닌 패키지, 부속 파일들이 삭제되지않고 찌꺼기처럼 쌓이는 경우가 있음.

아마 위의 찌거기로 인해 mysql이 새로 설치되는게 아닌 찌꺼기를 참고하는 느낌을 받았음.

- brew cleanup을 통해 깔끔하게 청소할 수 있음.

brew remove mysql<br>
brew cleanup

sudo rm -rf /opt/homebrew/var/mysql

brew install mysql

이후 mysql폴더의 권한을 부여함으로써 접속에 성공했음.

```
chmod -R 777 /opt/homebrew/var/mysql/
```
