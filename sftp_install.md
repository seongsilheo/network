# 파일 전송 통신 규약
- FTP(File Transfer Protocol): 파일을 전송하는 통신 규약. 기본 포트 21

- SFTP(Secure File Transfer Protocol): FTP에 보안기능이 추가. Ssh(Secure SHell)와 같은 방식을 이용하여 안전하게 암호화된 구간에서 FTP기능 사용. 

# sftp 설정방법
## 1. 설치된 패키지 업그레이드 
<br/>
![image](https://user-images.githubusercontent.com/44438752/62205527-95d46080-b3ca-11e9-967c-ce324467d7eb.png)

![스크린샷 2019-07-31 오후 7 06 54](https://user-images.githubusercontent.com/44438752/62203620-7b988380-b3c6-11e9-8337-ea32b845120a.png)
<br/><br/>
## 2. 설치된 패키지 리스트 확인
### - 여기서는 openssh-server가 설치되지 않았음을 확인할 수 있음
<br/>
![image](https://user-images.githubusercontent.com/44438752/62205588-be5c5a80-b3ca-11e9-96ec-f31045fd04d5.png)
<br/>
deb 파일 설치 : dpkg -i <file name.deb>
패키지 제거 : dpkg -P <package nae>
설치된 패키지 리스트: dpkg -l
설치된 패키지에 포함된 파일 보기 dpkg -L <package name>
deb 파일 포함된 파일들 보기 : dpkg -c <file name.deb>
deb 파일의 정보보기 : dpkg -l <file name.deb>
파일의 패키지명 알아내기: dpkg -S <file name>
grep openssh -> openssh라는 문자 검색
