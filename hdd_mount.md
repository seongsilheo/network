# 파티션 나누기 
mount하기 이전에 partition(공간)을 나눠줘야 mount 가능. 하드디스크 4개를 mount해야 할 경우,
os를 설치한 하드디스크 a를 제외하고 b,c,d는 파티션이 나눠져있지 않음. 

<br/><br/>
## 1. Disk 상태 보기
- sda 외에 sdb, sdc, sdd는 파티션이 잡혀있지 않음을 확인할 수 있음


![image](https://user-images.githubusercontent.com/44438752/62207187-7fc89f00-b3ce-11e9-990b-9e4f9d6a5058.png)

<br/><br/>
##2. 파티션 나누기 (여기서는 sbd 먼저 파티션 설정)


![image](https://user-images.githubusercontent.com/44438752/62207237-9969e680-b3ce-11e9-93a7-98bbc789cc45.png)
![image](https://user-images.githubusercontent.com/44438752/62207109-47c15c00-b3ce-11e9-96ae-36c764603e14.png)
![image](https://user-images.githubusercontent.com/44438752/62207270-ae467a00-b3ce-11e9-83d7-c1f50fae7ae3.png)

<br/><br/>
3. 포맷 설정(파일 저장 방법 설정)
- 혹 포맷 설정 안되면 이미 mount되어 있는지 확인하고, mount 되어 있으면 unmount 시킨 후에 포맷 설정할것
- ext4(리눅스 저널링 파일 시스템) 라는 형식으로 포맷 할 것이다.


![image](https://user-images.githubusercontent.com/44438752/62207320-cf0ecf80-b3ce-11e9-90fa-9a67f2ae8f47.png)

4. 부팅시 자동으로 하드디스크를 자동 mount하도록 설정
- /etc/fstab에 추가된 하드디스크 정보들 입력
- mi_hdd_1, mi_hdd_2, mi_hdd_3 폴더 먼저 생성하고 자동 마운트 설정

![image](https://user-images.githubusercontent.com/44438752/62207458-2614a480-b3cf-11e9-911f-5ec428990a28.png)
![image](https://user-images.githubusercontent.com/44438752/62207471-2ca31c00-b3cf-11e9-9858-a6ca4e648453.png)
