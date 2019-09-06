# Git Branch

Branch를 통한 코드 관리

시작은 master에서 함
first commit
브랜치 만듬(test)
아직 test도 master 와 함께 있음.
나중에 알게 되면 브랜치는 그저 포인터였을 뿐임.

## 깃을 알아야 하는 이유

- CI, CD 를 하기 위해서 깃을 기업들이 사용함.
- 깃은 각각의 브랜치를 다른 세계로 인식함.
  (평행우주 같이 인식) --> 가장 큰 장점
- 한 번 넘어가면 못 돌아옴

## Branch

1. `git branch`: 깃 브랜치 확인 
   깃 브랜치들을 알려주고 나의 위치를 알려줌
2. `git branch [브랜치명]`: 브랜치 생성 명령문
3. `git switch [브랜치명]`: 브랜치 전환

## Merge 시나리오

1. fast-forward : 
   main이 될 애를 찾음(=master)
   new는 곁가지 

main입장에서 합병하는 느낌
내가 흡수를 할 애로 이동함 (main이 )
merge 중 가장 쉬운 merge

2. Auto-merge(merge without conflict)
3. Merge with Conflict

## Conflict 발생 

1. 이젠 conflict가 날거야 같은 줄을 수정했으니(master에서 작성)
2. 이건 conflict 브랜치에서 작성