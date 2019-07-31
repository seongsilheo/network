## 1. 폴더 권한 확인
         d /  rwxr-xr-x/ 2/ root / root / 4096 / Apr 22 16:59 / seongsil

     파일Type 퍼미션정보 링크수 소유자 소유그룹  용량     생성날짜        파일이름
     
- r: 파일의 읽기 권한 <br/>
- w: 파일의 쓰기 권한 <br/>
- x: 파일의 실행 권한 <br/>
<br/>
- 퍼미션 정보: 앞에서 세자리씩 끊어서, 소유자:rwx 그룹:r-x, 공개:r-x

![image](https://user-images.githubusercontent.com/44438752/62207990-9243d800-b3d0-11e9-83bf-a6e38d8c213e.png)
<br/><br/>

## 2. 유저, 그룹 추가

- seongsil이라는 유저 추가 <br/>
![image](https://user-images.githubusercontent.com/44438752/62208031-a982c580-b3d0-11e9-93fa-d8a4c2f0b54c.png)

- seongsil 유저는 그룹 group1에 추가
![image](https://user-images.githubusercontent.com/44438752/62208033-abe51f80-b3d0-11e9-926e-d45d17b56657.png)


<br/><br/>

## 2. 폴더 권한 설정
- 퍼미션 변경하고 싶을 때는 chmod [변경된 퍼미션값] [변경할 파일]
- r=4, w=2, x=1로 4+2+1 | 4+1+ 1 | 4 + 2 + 1 로 권한 변경을 하고 싶으면 변경된 퍼미션 값에 767 입력. -R 옵션은 하위 디렉토리의 모든 디렉토리/파일의 퍼미션이 변경.
- 소유자 변경은 chown [변경할 소유자] [변경할 파일]
- 여기서 mi_hdd_1 폴더 권한 설정

![image](https://user-images.githubusercontent.com/44438752/62207972-85bf7f80-b3d0-11e9-9415-d46eaae5bce2.png)


- 폴더의 사용자와 그룹 수정


![image](https://user-images.githubusercontent.com/44438752/62208216-2615a400-b3d1-11e9-97cd-d094df15bea8.png)


<br/><br/>

## 3. 외부에서 테스트
- 테스트 이전에 sftp 서버 먼저 설치할 것
https://github.com/seongsilheo/network/blob/master/sftp_install.md

![image](https://user-images.githubusercontent.com/44438752/62208267-4b0a1700-b3d1-11e9-964f-7a7395c4d4ab.png)
