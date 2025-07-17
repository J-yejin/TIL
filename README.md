# TIL (About GIT)

### What is git
#### GIT : 분산 버전 관리 시스템
코드 변경 이력을 기록하고 협업을 원활하게 하는 도구

- working directory
- staging area
- repository

### main code
- add : working directory -> staging area로 이동
```python
git add file_name
```

- commit : staging area로 이동한 파일에 대한 메세지 기록 -> 버전 관리 시 변경사항 기록
```python
git commit
```
1. 이 상태에서 I 눌러 insert 상태로 만들어 vim에 입력
2. 이후 esc 눌러 insert 해제
3. :wq 입력해 저장하고 나가기
=> commit message 입력 완료

- push : staging area -> repository로 보내는 것
```python
git remote add origin remote_repo_url
git push origin master
```
1. repo를 로컬과 연결
   - origin : alias, repo의 별칭
   - remote_repo_url : 깃 주소
2. 해당 코드는 첫번째 push에서 사용

```python
git push --set-upstream origin master
```
이렇게 하면 origin master에 push 하도록 기본적 세팅 가능

- pull & clone
   - clone : 원격 저장소 전체를 복제해서 git > local
   - pull : git 상의 변경사항만 local로 가져오는 것

  ** 협업 시 가장 먼저 pull을 해서 변경사항 확인하기!


### commit하지 않으면 push 할 수 없다!!
### add > commit > push 순서 기억


#### 그 외 알고 있으면 유용한 code
- git status : git의 현재 상태 확인
- git log : commit 내역 확인

