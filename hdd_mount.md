# 파티션 나누기 
mount하기 이전에 partition(공간)을 나눠줘야 mount 가능. 하드디스크 4개를 mount해야 할 경우,
os를 설치한 하드디스크 a를 제외하고 b,c,d는 파티션이 나눠져있지 않음. 

1. Disk 상태 보기
- sda 외에 sdb, sdc, sdd는 파티션이 잡혀있지 않음을 확인할 수 있음


![image](https://user-images.githubusercontent.com/44438752/62207187-7fc89f00-b3ce-11e9-990b-9e4f9d6a5058.png)
2. 파티션 나누기 (여기서는 sbd 먼저 파티션 설정)


![image](https://user-images.githubusercontent.com/44438752/62207237-9969e680-b3ce-11e9-93a7-98bbc789cc45.png)
![image](https://user-images.githubusercontent.com/44438752/62207109-47c15c00-b3ce-11e9-96ae-36c764603e14.png)
![image](https://user-images.githubusercontent.com/44438752/62207123-50b22d80-b3ce-11e9-8929-fa9cfae03652.png)
