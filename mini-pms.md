## init
- [~]$ mkdir mini-pms
- [~]$ cd mini-pms
- [~/mini-pms]$ gradle init
    - gradle 버전 차이때문인지 여기서 예전하고 다름
        ```console
        Split functionality across multiple subprojects?:
        1: no - only one application project
        2: yes - application and library projects
        Enter selection (default: no - only one application project) [1..2] 1
        ```
        - app폴더가 생김(그 안에 src폴더랑 build.gradle 있음)
        - settings.gradle에 include('app')가 추가되었음
        - build.gradle plugins에 java가 없음, 그래서 임의로 추가했음
        - jcenter에서 mavenCentral로 바뀜
- [~/mini-pms]$ gradle build
- [~/mini-pms]$ tree

```groovy
plugins {
    id 'java'
    id 'application'
    id 'eclipse'   <== 이 코드를 추가한다.
}
```

- gradle eclipse
- git init
- .gitignore
- git add .
- git commit -m "프로젝트 준비"
- github 에 원격 저장소 생성
- git remote add [원격저장소이름] [원격저장소URL] (보통 origin으로 한다)
- git remote
- git remote -v
- git push -u [원격저장소이름] [로컬브랜치]:[원격브랜치] (origin master:master)

## 이클립스 단축키
- alt+shift+x -> j