# 빅데이터

## 빅데이터란?
- 기관 또는 조직들이 생성하는 방대한 규모의 복잡한 데이터 묶음
    
- A Field that Treats way to Analyze
    - 거대한 데이터를 분석하는 방법을 다루는 어떤 분야
    
- Systematucally Extract Information
    - 시스템적으로 정보를 어디선가 추출 데이터 묶음을 분석하는 과정

### Data Sets : A Collection of Data
- 데이터 셋 : 

수집 된 데이터들의 집합 혹은 조합을 의미
다양한 형태로 만들어지며 행과 열 형태로 구성
빅데이터는 통합적이며 포괄적인 데이터
- 어느 한 부분의 데이터가 아닌 전체적인 데이터를 수집하여 연구

### 빅데이터의 특징
- 3V : 규모(Volume), 다양성(variety), 속도(Velocity)
- 5V : 규모(Volume), 다양성(variety), 속도(Velocity), 정확성(Veracity), 가치(value)

    - **규모(Volume)** : 기업이 관리하고 분석하는 빅 데이터 크기와 양
    - **가치(Value)** : 비즈니스 관점에서 가장 중요한 "V"인 빅데이터의 가치는 일반적으로 보다 효과적인 운영, 더 강력한 고객 관계 및 기타 명확하고 수량화 가능한 비즈니스 이점으로 이어지는 통찰력 발견 및 패턴 인식에서 나옵니다.
    - **다양성(Variety)** : 비정형 데이터, 반정형 데이터 및 원시 데이터를 포함하는 다양한 데이터 유형
    - **속도(Velocity)** : 회사가 데이터를 수신, 저장 및 관리하는 속도
        - (예: 특정 기간 내에 수신된 특정 소셜 미디어 게시물 또는 검색 쿼리 수)
    - **진실성(Veracity)** : 종종 경영진들의 신뢰도에 영향을 미치는 데이터 및 정보 자산의 "진실" 또는 정확성

- *Data Types*
    - 정형 데이터 (Structured Data)
        - 틀이 잡혀있는, 체계화 된 데이터로 우리가 흔히 엑셀에 정리된 자료를 생각하면 된다. 이미 해당 자료 수집 목적에 맞게 정리된 데이터 이기에 데이터 분석에 용이한 자료 형태이다.
    - 비정형 데이터 (Unstructured Data)
        - 구조화 되지 않은 데이터로 텍스트, 그림, 비디오 등이 있으며, 추가적인 분석을 위해서는 구조화된 형태로 변환해야 한다.
    - 반정형 데이터 (Semi-Structured Data)
        - HTML, JSON, Log 형태가 대표적으로 흔히 정형 데이터와 같은 구조의 정리된 데이터 모델을 준수하진 않지만 태그와 기타 마커 등을 통해 데이터 내의 레코드와 필드 계층이 구분된 데이터이다.
    - 원시 데이터 (Raw Data) 
        - 가공되지 않은 형태의 데이터를 가르키는데, 이는 일반적으로 데이터가 수집되거나 생성된 직후의 형태를 말한다. 원시 데이터는 일반적으로 구조화되지 않고, 정제되지 않은 상태이며, 처리되지 않은 형태입니다.
            - (예: 로그데이터, 센서 데이터, 이미지 및 비디오, 텍스트 데이터)

### 빅데이터를 활용한 사례들
- 페이팔, 사기 막기 위해 딥러닝 도입
- MLB, NFL에 빼앗긴 시장 되찾기 위해 빅데이터 도입
- GE(General Electric)
- 금융권
- [[사례들의 출처]](https://www.elec4.co.kr/article/articleView.asp?idx=15220)

## Hadoop (하둡)
- **Hadoop 이란?**
    - 대규모 데이터 집합을 분산 처리하는 데 사용되는 자바 기반의 오픈 소스 프레임워크
    - Apache Software Foundation에서 개발되었고, 대용량 데이터를 처리하고 저장하기 위한 여러 가지 도구와 라이브러리를 제공하며 이걸 Hadoop 생태계(Hadoop Ecosystem)라고 한다.
- **Hadoop의 특징**
- 장점
    - *용이한 확장성*
        - 새로운 노드를 클러스터에 추가하여 시스템을 확장할 수 있으며, 처리량과 저장 용량을 필요에 따라 증가시킬 수 있다.
        - **클러스터란?**
            - 특정한 기능 수행을 위해 여러 대의 컴퓨터가 네트워크로 연결된 것을 의미하며, 이때 클러스터를 구성하는 개별 컴퓨터를 node라고 칭한다.
    - *저비용*
        -  오픈 소스로 제공되어 라이센스 비용이 없으며, 저렴한 컴퓨팅 자원을 활용하여 비용을 절감
    - *고용량 저장*
        - 대용량 데이터를 저장할 수 있는 분산 파일 시스템인 HDFS를 사용하여 데이터를 안전하게 저장하고 관리할 수 있습니다.
    - *유연한 데이터 처리*
        - 다양한 종류(정형, 비정형, 반정형)의 데이터를 처리할 수 있으며, MapReduce와 같은 프레임워크를 사용하여 데이터를 분석하고 처리할 수 있습니다.
        - 구조화된 데이터부터 비구조화된 데이터까지 다양한 형식의 데이터를 효과적으로 처리
    - *고가용성*
        - 데이터를 여러 복제본으로 저장하여 데이터의 손실을 방지하고
        , 노드나 컴퓨터의 고장에 대비하여 데이터를 안전하게 보호
    - *설치와 관리의 용이성*
        - 상대적으로 쉬운 설치 및 관리 프로세스를 가지고 있어,
        기업이 빠르게 환경을 구축하고 운영
    - *강력한 생태계*
        - 하둡 생태계에는 많은 다양한 도구와 프레임워크가 있으며, 이를 통해 빅데이터를 분석하고 인사이트를 추출할 수 있습니다.
        (예: HBase, Hive, Pig, Spark, Kafka 등)
        ![default](/이미지%20파일/하둡의%20생태계.png)
- 단점
    - HDFS에 저장된 데이터를 변경 불가
    - 실시간 데이터 분석 같이 신속하게 처리해야 하는 작업에는 부적합
    - 너무 많은 버전과 부실한 서포트
    - 설정의 어려움
### 하둡의 구성요소 (Hadoop Stack)
- *하둡 분산형 파일시스템(Hadoop Distributed File System, HDFS)*
    - 하둡 네트워크에 연결된 기기에 데이터를 저장하는 분산형 파일 시스템
#### **Hadoop HDFS**
- 데이터를 저장하면, 다수의 노드에 복제 데이터도 함꼐 저장해서 데이터 유실을 방지
- 대용량 데이터를 분산하여 저장하는 파일 시스템
- 대용량 데이터를 블록(block)으로 분할하여 저장하며, 데이터 처리 작업에 있어서 중요한 역할
##### **Hadoop HDFS Architecture**
- HDFS는 마스터 슬레이브 구조로 하나의 네임노드와 여러 개의 데이터노드로 구성됩니다. 네임노드는 메타 데이터를 가지고 있고, 데이터는 블록 단위로 나누어 데이터노드에 저장된다. 사용자는 네임노드를 이용해 데이터를 쓰고, 읽을 수 있다.
(![alt text](/이미지%20파일/Hadoop%20HDFS%20Architecture.png))

1. 블록 구조의 파일 시스템으로, 저장하는 파일은 특정 사이즈의 블록으로 나누어져 분산된 서버에 저장됨.
2. 하나의 블록은 3개 (수정 가능)로 복제되며, 각각 다른 HDFS의 노드에 분산 저장됨 (**Replication**)
3. HDFS에는 마스터 역할을 하는 네임노드 서버 한 대와, 슬레이브 역할을 하는 데이터 노드 서버가 여러 대로 구성된다.
4. 네임 노드는 HDFS의 모든 메타데이터(블록들이 저장되는 디렉토리
의 이름, 파일명등.)를 관리하고, 클라이언트가 이를 이용하여 HDFS
에 저장된 파일에 접근할 수 있다.
5. 하둡 어플리케이션은 HDFS에 파일을 저장하거나, 저장된 파일을 읽
기 위해 HDFS 클라이언트를 사용하며, 클라이언트는 API형태로 사
용자에게 제공된다.
6. 데이터 노드는 주기적으로 네임노드에서 블록 리포트(노드에 저장되
어 있는 블록의 정보)를 전송하고 이를 통해 네임노드는 데이터 노드
가 정상 동작하는지 확인. (**Heartbeats**)
7. 클라이언트는 네임노드에 접속해서 원하는 파일이 저장된 블록의 위
치를 확인하고, 해당 블록이 저장된 데이터 노드에서 직접 데이터를
조회함.

- 네임노드
    - 네임노드의 주요 역할은 메타데이터 관리와 데이터노드의 관리

    - 메타데이터 관리
        - 메타데이터는 파일이름, 파일크기, 파일생성시간, 파일접근권한, 
        파일 소유자 및 그룹 소유자, 파일이 위치한 블록의 정보 등으로 구성된다.
        각 데이터노드에서 전달하는 메타데이터를 받아서 전체 노드의 메타데이터
        정보와 파일 정보를 묶어서 관리합니다.
            
        - 메타 데이터는 사용자가 설정한 위치에 보관된다. 네임노드가 실행 될 때
        파일을 읽어서 메모리에 보관하고, 운영중 발생한 수정사항은 네임노드의 메모리에
        바로 적용된 후 수정사항을 다음 구동 시 적용을 위해서 주기적으로 Edist 파일로 저장.

    - 메타데이터 파일 종류
        - Fsimage 파일
            - 네임스페이스와 블록 정보
        - Edits 파일
            - 파일을 생성, 삭제에 대한 트랜잭션 로그
            - 메모리에 저장하다가 주기적으로 생성

    - 메타데이터 파일 저장 형태
        - 사용자가 설정한 위치 (dfs.name.dir)에 다음과 같은 파일의 형태로 저장된다.
        ![default](/이미지%20파일/메타데이터%20형태.png)

        - **메타데이터**
            - VERSION : 현재 실행 중인 HDFS의 ID, 타입 등 정보
            - `edits_0000xxx-0000xxx` : 트랜잭션 정보. edits_트랜잭션시작번호-트랜잭션
            종료번호 까지의 정보를 저장 
            - `edits_inprogress_000xx` : 최신 트랜잭션 정보. 압축되지 않은 정보
            - `fsimage_000xxx` : 000xxx 까지 트랜잭션 정보가 처리된 fsimage
            - `seen_txid` : 현재 트랜잭션 ID
        
    - 데이터노드 관리
        - 네임노드는 데이터노드가 주기적으로 전달하는 하트비트(3초, dfs.heartbeat.interval)와 블록리포트(6시간, dfs.blockreport.intervalMsec)를 이용하여 데이터 노드의 동작상태, 블록상태를 관리합니다.

        
    - **데이터노드**
        - 데이터노드는 파일을 저장하는 역할을 한다. 파일은 블록단위로 저장하고, 주기적으로 네임노드에 하트비트와 블록리포트를 전달한다. *하트비트*는 데이터노드의 동작여부를 판단하는데 이용된다. 네임노드는 하트비트가 전달되지 않는 데이터노드는 동작하지 않는 것으로 판단하여 더 이상 데이터를 저장하지 않도록 설정한다. *블록리포트*로 블록의 변경사항을 체크하고, 네임노드의 메타데이터를 갱신한다.

##### HDFS 세이프모드
- HDFS의 세이프모드(safemode)는 데이터 노드를 수정 할 수 없는 상태이다. 세이프 모드가 되면 데이터는 읽기 전용상태가 되고, 데이터 추가와 수정이 불가능하면 데이터 복제도 일어나지 않는다. 관리자가 서버 운영 정비를 위해 세이프 모드를 설정 할 수도 있고, 네임노드에 문제가 생겨 정상적인 동작을 할 수 없을 때 자동으로 세이프 모드로 전환된다.

- 세이프 모드 커맨드
![default](/이미지%20파일/세이프모드%20커맨드.png)

- 복구
    - HDFS 운영 중 네임노드 서버에 문제가 생겨서 세이프 모드에 진입하는 경우는 네임노드 자체의 문제와 데이터 노드의 문제일 경우가 많다.

    - fsck 명령으로 HDFS의 무결성을 체크하고, hdfs dfsadmin -report 명령으로 각 데이터 노드의 상태를 확인하여 문제를 확인하고 해결한 후 세이프 모드 해제

##### HDFS 휴지통
- HDFS는 사용자의 실수에 의한 파일 삭제를 방지하기 위해서 휴지통 기능을 제공한다.
- 휴지통 기능이 설정되면 HDFS에서 삭제한 파일은 바로 삭제되지 않고, 각 사용자의 홈 디렉토리 아래 휴지통 디렉토리(/user/유저명/.Trash)로 이동된다. 휴지통 아래의 파일은 복구할 수 있다.
- 휴지통 디렉토리는 지정한 간격으로 체크포인트가 생성되고, 유효 기간이 만료되면 체크포인트를 삭제한다. 삭제 되면 해당 블록을 해제하고, 사용자에게 반환한다.

*휴지통 설정*
- ![default](/이미지%20파일/휴지통%20설정.png)
- core-site.xml에 아래와 같이 설정
- ![default](/이미지%20파일/휴지통설정2.png)

##### HDFS 명령어
- **사용자 커맨드**
    - 사용자 커맨드는 hdfs, hadoop 쉘을 이용할 수 있습니다. 일부 커맨드는 hdfs 쉘을 이용해야 합니다. 둘 다 이용할 수 있는 경우 각 쉘의 결과는 동일하다.
    - ![default](/이미지%20파일/HDFS%20사용자%20공용커맨드.png)

    - 사용자 커맨드 목록
    - ![default](/이미지%20파일/사용자%20커맨드%20목록.png)

    - **dfs 커맨드**
        - dfs 커맨드는 파일시스템 쉘을 실행하는 명령어이다. dfs는 hdfs dfs, hadoop fs, hadoop dfs 세가지 형태로 실행이 가능하다. 

        1. ls
            - 하둡 파일 디렉토리 내의 파일들을 화면에 출력하는 명령어, 기본값으로 이름별로 출력
            - 주요옵션: -h, -R,-u
            ```
            $ hadoop fs -ls /user/
            # 사람이 읽을 수 있는 형태로 파일사이즈를 메가, 기가로 변경하여 출력 
            $ hadoop fs -ls -h /user/
            # 하위 폴더까지 조회 
            $ hadoop fs -ls -R /user/
            # 액세스 시간을 조회. 기본설정은 생성 시간. 마지막 접근 시간을 확인하여 파일 정리 가능 
            $ hadoop fs -ls -u /user/

            ```
        2. mkdir
            - 다양한 옵션별로 디렉토리를 만들 수 있는 명령어
            - 주요옵션: -p
            ```           
            $ hadoop fs -mkdir /user/folder
            /user/folder1/folder2를 생성, 상위 폴더가 없으면 자동으로 생성 
            $ hadoop fs -mkdir -p /user/folder1/folder2
            ```
        3. touchz
            - 0byte 파일 (빈 라인 곧 빈 데이터 길이)의 파일 생성
            ```
            ~/hadoop$ hadoop fs -touchz /user/hadoop-test.txt
            ~/hadoop$ bin/hdfs dfs -touchz /hdfs-user/test.txt
            ```
        4. put
            - 하나의 파일이나 디렉토리 내의 모든 파일들을 리눅스 로컬 파일 시스템에서 해당 목적지 하둡 파일 시스템의 소스로 복사하는 명령어
            - 주요옵션: -f
            ```
            $ hadoop fs -put ./data1.txt /user/
            동일한 이름의 파일이 존재하면 덮어씀 
            $ hadoop fs -put -f ./data1.txt /user/
            ```
        5. copyFromLocal
            - put 명령어와 비슷하지만 소스는 로컬 파일 참조를 위해 제한적
            ```
            ~/hadoop$ bin/hdfs dfs -copyFromLocal /etc/apt/ /user/etc/apt
            ```
        6. get
            - 하둡 분산 파일 시스템에서 리눅스 로컬 파일 시스템으로 복사
            - CRC(Cyclic Redundancy Check) 체크실패여부 관련 파일을 복사
            - CRC : 전송된 데이터의 오류 여부를 체크하는 값
            - 주요옵션: -f
            ```
            $ hadoop fs -get /user/data1.txt ./
            # 동일한 이름의 파일이 존재하면 덮어씀 
            $ hadoop fs -get -f /user/data1.txt ./
            ```
        7. copyToLocal
            - get 명령어와 비슷하지만, 목적지가 로컬 파일 참조로 제한
            ```
            ~/hadoop$ bin/hdfs dfs -copyToLocal /user/hadoop-test.txt /tmp
            ```
        8. cat
            - hdfs url 상의 파일이나 해당 파일을 stdout(화면 출력)으로 찍어 보여주며 이는 리눅스 cat 명령어와 동일
            ```
            ~/hadoop$ bin/hdfs dfs -cat /user/etc/xml/docbook-xml.xml
            ```
        9. mv
            - hdfs 내부 하둡 분산 시스템 내에서 파일을 옮길 수 있다.
                로컬 시스템으로는 불가
            ```
            ~/hadoop$ hadoop fs -mv /user/etc/apt/ /user/etc/xml
            ```
        10. cp
            - hdfs 내부 하둡 분산 시스템 내에서 파일을 복사할 수 있다.
                로컬 시스템으로는 불가
            ```
            ~/hadoop$ bin/hdfs dfs -cp /user/etc/xml/apt/ /user/etc/
            ```
        11. rm
            - hdfs 파일 내부에 특정 폴더나 파일을 삭제
            - 주요 옵션: -R
            ```
            $ hadoop fs -rm /user/data1.txt 
            # 디렉토리를 포함하여 하위의 모든 파일을 삭제, 디렉토리 삭제시 필요함 
            $ hadoop fs -rm -r /user/
            # 쓰레기통을 사용하지 않고 파일 삭제  
            $ hadoop fs -skipTrash /user/
            ```
        12. chmod 
            - 해당 파일의 owner(소유자) 혹은 super owner일 경우 그 파일의 권한을 읽고 쓰고 삭제 수정하는 권한을 수정 및 적용
            ```
            ~/hadoop$ hadoop fs -chmod -R 755 /user/etc/xml
            ```
        13. chown
            - 해당 파일의 Super Owner일 경우 그 파일의 owner(소유자)를 변경하여 수정
            ```
            ~/hadoop$ hadoop fs -chown root /user/etc/xml
            ```
        14. setrep
            - 디렉토리, 파일의 레플리케이션 팩터를 수정합니다.
            - 주요옵션: -R
            ```
            # 디렉토리의 복제개수를 5로 설정  
            $ hadoop fs -setrep 5 /user/
            # 하위의 모든 디렉토리, 파일의 복제개수를 5로 설정 
            $ hadoop fs -setrep 5 -R /user/
            ```
        15. test
            - 파일, 디렉토리의 존재 여부를 확인합니다.
            ```
            # -d: 경로가 디렉토리이면 0을 반환합니다.
            # -e: 경로가 있으면 0을 반환합니다.
            # -f: 경로가 파일이면 0을 반환합니다.
            # -s: 경로가 비어 있지 않으면 0을 반환합니다.
            # -w: 경로가 존재하고 쓰기 권한이 부여 된 경우 0을 반환합니다.
            # -r: 경로가 존재하고 읽기 권한이 부여 된 경우 0을 반환합니다.
            # -z: 파일 길이가 0이면 0을 반환합니다.

            # /user/test.txt 파일이 존재하면 0을 반환 
            $ hadoop fs -test -e /user/test.txt
            ```
        16. stat
            - 주어진 포맷에 따른 파일의 정보를 확인한다.
            ```
            # 주요 포맷
            # %y : 마지막 수정 시간 
            # %x : 마지막 접근 시간 
            # %n : 파일 이름 
            # %b : 파일 사이즈 (byte)
            $ hadoop fs -stat "%y %n" hdfs://127.0.0.1:8020/*
            ```
        17. setfacl
            - 파일의 ACL을 설정합니다. ls 명령으로 확인할 수 있는 파일의 권한과 별도로 권한을 설정할 수 있다.
            ```
            # -m: 권한을 수정
            # -b: 설정한 권한을 삭제 
            # user a에게 /user/file의 읽기(r), 쓰기(w) 권한을 줌
            $ hadoop fs -setfacl -m user:a:rw- /user/file

            # /user/file에서 신규로 생성되는 파일, 디렉토리에 대하여 user a에게 의 읽기(r), 쓰기(w) 권한을 줌
            $ hadoop fs -setfacl -m default:user:a:rw- /user/file
            ```
        18. getfacl
            - 파일의 ACL을 확인한다.
            ```
            $ hadoop fs -getfacl /user/file
            # file: hdfs:///user/file
            # owner: c
            # group: g
            user::rw-
            user:a:rw-
            group::r--
            mask::rw-
            other::---
            ```
        19. count
            - 지정한 경로의 디렉토리 개수, 파일개수, 파일 사이즈 확인한다. -q, -v 옵션과 함꼐 사용하여 더 많은 정보 확인 가능
            ```
            # 디렉토리 개수 150
            # 파일 개수 2000
            # 디렉토리 용량 123456789
            $ hadoop fs -count /user
                150      2000     123456789 hdfs:///user

            # -h 사용자가 읽기 편하게 변환
            # -q 디렉토리의 쿼터 정보 확인: QUOTA, REMAINING_QUOTA, SPACE_QUOTA, REMAINING_SPACE_QUOTA, DIR_COUNT, FILE_COUNT, CONTENT_SIZE, PATHNAME
            # -u 디렉토리의 쿼터 정보 확인: QUOTA, REMAINING_QUOTA, SPACE_QUOTA, REMAINING_SPACE_QUOTA, PATHNAME
            # -v는 -q, -u와 함께 사용하면 헤더를 함께 출력합니다. 
            $ hadoop fs -count -q -v hdfs:///user/sample
                QUOTA       REM_QUOTA     SPACE_QUOTA REM_SPACE_QUOTA    DIR
                _COUNT   FILE_COUNT       CONTENT_SIZE PATHNAME
                    8000000          471204 109951162777600  99303499783522       
                286862      7241934      3549220998026 hdfs:///user/sample
            ```
    - **Hadoop의 관리와 운영**
        1. archive
            - 하둡 에코시스템에서 사용되는 압축된 통합 파일 형식
            - 많은 수의 작은 파일을 하나의 아카이브 파일로 압축하여 대용량 파일 관리의
            오버헤드를 줄이는 데 사용
            - 하둡 분산 파일 시스템(HDFS) 또는 유사한 저장 시스템에서 많은 작은 파일로 이루어진
            데이터를 저장할 때 특히 유용
            - **하둡 아카이브의 작동 방식**
                1. 통합
                    - HAR은 작은 파일의 집합을 하나의 큰 파일로 통합하여 저장되는
                    파일의 총 수를 줄입니다.
                    - 통합은 많은 파일을 저장하고 관리하는 데 따르는 *오버헤드*를 최소화하는 데 도움
                    - 오버헤드 : 어떤 처리를 하기 위해 들어가는 간접적인 처리 시간, 메모리 등
                2. 압축
                    - HAR 파일은 일반적으로 압축되어 있으며, 이는 필요한 저장 공간을 줄이고 데이터
                    전송 효율을 향상시킴
                3. 메타데이터
                    - HAR 아카이브는 포함된 파일에 대한 메타데이터 정보를 저장하여 아카이브 내의 개별 파일을 효율적으로 조회하고 검색할 수 있도록 합니다.
                    - 메타데이터 : 아카이브 파일 내의 파일 구조, 위치 및 기타 정보
                4. 엑세스 최적화
                    - 하둡과 같은 분산 컴퓨팅 환경에서 네트워크 및 디스크 I/O가 중요한 병목 현상이
                    될 수 있는 경우 HAR 파일에 저장된 데이터에 엑세스하는 것은 동일한 데이터를 여러
                    작은 파일로 분산된 상태에서 엑세스하는 것보다 더 효율적일 수 있습니다.
        2. checknative
            - 하둡 네이티브 코드 가능성을 체크하는 것
            - Hadoop이 사용하는 네이티브 라이브러리들의 버전과 구성을 출력
            - 시스템에서 Hadoop이 정상적으로 작동하기 위해 필요한 네이티브 라이브러리들이 올바르게 설치되어 있는지 확인
        3. classpath
            - 하둡의 클래스 경로를 출력하는 명령어이다주로 하둡 JAR 파일이나 다른 리소스를 실행할 때
            필요한 클래스 경로를 확인할 때 사용된다.
        4. conftest
            - 하둡의 xml 설정 파일 구성을 검증하기 위한 사용자 명령어
            - 검증 방법은 해당 xml 파일을 파싱하고 이중성 검증과 빈 속성 이름들을 체크하여 검증
        5. credential
            - Hadoop 클러스터에서 봉안과 관련된 정보를 저장하고 관리하는 데 사용되는 메커니즘
            - 보안 토큰, 비밀번호, 인증서 등이 포함
            - 하둡과 하둡 에코시스템 간에 보안으로 연결
        6. distcp
            - 한번에 많은 파일들의 권한과 소유자를 변경할 수 있는 사용자 명령어
        7. fs
            - HDFS 파일 시스템을 조작하는 명령어
            - 분산된 클러스터 간에 데이터를 효율적으로 이동하고 복제할 때 사용
        8. jar
            - 하둡의 어플리케이션을 실행시키거나 혹은 Yarn/MapReduce 어플리케이션을 실행하는 명령어
        9. kerbname
            - 보안 규칙(auth_to_local 규칙)을 적용하여 Kerberos 주체를 Hadoop 사용자 이름으로 매핑할 때 사용
        10. kdiag
            - kerberos 티켓 캐시, 키 탭 및 기타 인증 구성을 검사하고 문제를 식별하는 데 도움
        11. version
            - 하둡 버전에 대한 정보를 출력
        12. envvars
            - 하둡의 환경변수를 디스플레이하도록 도와주는 사용자 명령어
#### **MapReduce**
- 대규모 데이터 집합을 처리하는 분산 프로그래밍 모델 및 프레임워크
- 데이터를 여러 노드에 분산하여 병렬로 처리하고, 각 노드에서의 작업 결과를
모아 최종 결과를 생성
- 주로 데이터의 필터링, 정렬, 그룹화, 집계 등의 작업에 사용

    **Map**
    - 흩어져 있는 데이터를 연관성 있는 데이터들로 분류하는 작업(Key, Value의 형태)

    **리듀스(Reduce)**
    - Map에서 출력된 데이터를 중복 데이터를 제거하고 원하는 데이터를 추출하는 작업

    - ![alt text](/이미지%20파일/image-2.png)
    1. Splitting : 문자열 데이터를 라인별로 나눈다.
    2. Mapping : 라인별로 문자열을 입력받아, <key, value> 형태로 출력.
    3. Shuffling : 같은 key를 가지는 데이터끼리 분류.
    4. Reducing : 각 key 별로 빈도수를 합산해서 출력.
    5. Final Result : 리듀스 메소드의 출력 데이터를 합쳐서 하둡 파일 시
    스템에 저장.

#### YARN(Yet Another Resource Negotiator)
- 클러스터의 자원 관리 및 작업 스케줄링을 담당하는 클러스터
관리 시스템
- 클러스터의 자원을 애플리케이션에 할당하고, 각 애플리케이션
의 실행을 관리
- 다양한 유형의 응용 프로그램을 실행하고 자원을 효율적으로
활용할 수 있도록 지원

**YARN**
- Hadoop 2.x 버전부터 소개되었으며, 이전 버전의 Hadoop 
MapReduce에서 사용되던 장애 복구 및 작업 스케줄링을 분리하여
더욱 유연한 클러스터 리소스 관리를 제공
- MapReduce의 단점을 극복하기 위해 시작된 프로젝트

1. **자원 관리(Resource Management)**
    - 클러스터의 물리적 자원(메모리, CPU 등)을 애플리케이션에 동적으로 할당하
    여 관리
    - 클러스터의 자원 사용률을 최적화하여 다양한 유형의 애플리케이션을 동시에
    실행할 수 있도록 합니다.

2. **작업 스케줄링(Job Scheduling)**
    - 다양한 유형의 작업(예: MapReduce 작업, Spark 작업 등)을 효율적으
    로 스케줄링하여 클러스터 자원을 최대한 활용합니다.
    - 여러 작업이 동시에 실행될 수 있도록 작업을 우선 순위에 따라 관리
    합니다.
3. **확장성 (Scalability)**
    - YARN은 클러스터의 크기를 수평으로 확장할 수 있도록 설계
    - 새로운 노드가 추가되면 자동으로 클러스터에 추가됩니다
4.  **유연성 (Flexibility)**
    - 다양한 유형의 애플리케이션을 실행할 수 있는 유연성을 제공
    - MapReduce, Spark, Tez 등 다양한 프레임워크와 도구를 지원
5. **고가용성 (High Availability)**
    - 클러스터의 중요한 부분을 여러 개의 노드에 분산하여 장애 복구 지원

#### hadoop common-Libaraies and Utilites
- Hadoop 프레임워크의 기본 기능을 제공하고 클러스터에서 작업
을 관리하는 데 도움이 되는 다양한 도구
- Hadoop 클러스터를 구축하고 관리하는 데 필요한 핵심 기능을
제공

**1. hadoop-common.jar**
- Hadoop 클러스터의 다른 모든 구성 요소에 공통으로 사용되는
    핵심 유틸리티 및 기능을 제공
- HDFS, MapReduce 및 기타 하둡 구성 요소의 기본 클래스 및
    인터페이스를 포함

**2. hadoop-auth.jar**
- Hadoop 보안 관련 라이브러리입니다. 이를 사용하여 사용자 인
증 및 권한 부여를 관리하고, 보안 기능을 활성화할 수 있습니다

**3. hadoop-common-tests.jar**
- Hadoop Common 코드의 유효성을 검증하고 테스트

**4. bin/hadoop**
-  Hadoop 클러스터를 시작하고 관리하기 위한 명령줄 인터페이스
- 다양한 하둡 커맨드를 실행하여 HDFS 파일 시스템 및 MapReduce
작업을 관리

**5. sbin/start-dfs.sh 및 sbin/stop-dfs.sh**
- DFS 데몬을 시작하고 중지하기 위한 스크립트
- 클러스터의 HDFS 구성 요소를 시작하거나 중지할 때 사용

**6. bin/start-yarn.sh 및 sbin/stop-yarn.sh**
- YARN 데몬을 시작하고 중지하기 위한 스크립트
- 클러스터의 YARN 구성 요소를 시작하거나 중지할 때 사용

**7. sbin/start-all.sh 및 sbin/stop-all.sh**
- 클러스터의 모든 데몬을 한 번에 시작하거나 중지하는 스크립트
- HDFS 및 YARN 데몬을 모두 시작하거나 중지할 때 사용