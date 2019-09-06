# Git 기초

Git 기초 커맨드

- readme.md 로 프로젝트를 설명해줘야 함.(무조건 찍어주고 가기)
- 폴더 어떻게 운영할 지 readme에 정리(수칙,나와의 약속 등)
- 오자마자 친절하게 이 폴더에 뭐가 있는지 알려줘야 함.

1. 코드 관리 도구
   - SCM: Source Conde Message
   - VCS: Version control
2. 원격 저장소(git/github)
3. 협업 도구 
   - push & pull
   - forking & pull request
   - branching &request(github flow)



## 기본 커맨드

- `git init`: Git으로 프로젝트 관리 시작하겠다. (`.git` 폴더가 생김 

-> 망하면 .git을 지우면 됨.)
- `git add [파일명]`:staging
- `git status`: 상태 확인
- `git commit -m [메시지]`: commit
- `git log`:commit 히스토리


- git의 세 가지 상태 폴더
   - Staging area(index):

​      (사진대에 파일 추가하겠다.(git add  )
​      스냅샷 찍어서 올리는 곳)
​      언제든 이 곳으로 다시 돌아갈 수 있도록.
   - 특정 사진 찍는데 설명을 꼭 해줘야 함. 



해쉬함수: 어떤 값을 인자로 보내든지 2^160 자리의 수로 반환함 
디지털 세계의 암호화 담당함. 

깃에서 sha1을 쓴다.
-> 작은 변화도 금방 알아낸다. (해쉬 숫자값이 바뀌면 데이터가 변경되었음을 알아냄.)


깃 커밋 메세지: 
동사 목적어 형태로 쓰기 
합니다(동사원형) 무엇을~~


## 추가 커맨드
- `git checkout [커밋해시]`: 특정 commit을 확인하기
- `git restore [파일명]`:뭔가 새로 추가했는데 마음에 들지 않았다. (가장 최신 커밋으로 돌아가고 싶음.)

## 원격 저장소 관리(집에서 작업)
- `git remote`: 원격 저장소의 정보(이름)
- `git remote -v`: 원격 저장소의 정보(이름, 주소)
- `git remote add [이름] [주소]`: 원격 저장소 추가
- `git push [저장소 이름] [브랜치 이름]`: 원격 저장소 코드 업데이트
- `git clone [주소] [프로젝트 이름]`: 원격 저장소 코드 복제,
    깃으로 관리되는 애 밑에 깃 또 클론하면 안 됨(태양은 하나여야 한다. )
