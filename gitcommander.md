

## git commander

1.**new repository reset**

```
git init
```

- 여러 폴더에서 init해도 문제없음. 하지만, 중첩 폴더에서 하면 문제가 생길 수 있음



2.**원격 repo 복제**

```
git clone [URL]
```

3. **작업 폴더에서 변경 사항 확인**

```
git status
```

4. **변경된 파일 스테이징**

```
-특정 파일: git add [파일명]
-전체: git add .
```

5. **스테이징 내용 커밋**

```
git commit -m "msg"
```


6.**원격 저장소에 변경 puch**

```
git push orgin [브랜치명]
- 연결 ㅇ벗을 시: git remote add origin [url]
```

7. **변경사항 가져오기**

```
git pull origin [브랜치명]
```

## **브랜치 관리**

1. **브랜치 목록 확인**

```
git branch
```

2. **브랜치 생성 및 전환**

```
-생성 : git checkout -b [브랜치명]
-전환 : git checkout [브랜치명]
```

3. **브랜치 삭제**
 
```
git branch -d [브랜치명]
```

## git 사용시 주의사항

1. **git reset 주의하기**
   - `git reset --hard`는 작업 디렉토리의 변경사항을 모두 지움.
  
2. **작업하지 않은 변경 사항**
   - 다른 브랜치로 체크아웃 하기 전에 현재 브랜치의 변경사항을 커밋하거나 스테이징 해야함.

3. **git clean 주의**
   - 추적되지 않은 파일을 삭제함.
   - 실수로 중요한 파일을 삭제할 위험이 있음.

4. **백업**
   - git 저장소도 오류나 문제가 발생할 수 있으므로 주기적으로 백업하는 것이 좋음.

5. **`.gitignore`**
   - 불필요한 파일(로그,임시파일,중요 ip,id,pw)를 저장소에 포함되지 않도록 관리해야함.
  
6. 