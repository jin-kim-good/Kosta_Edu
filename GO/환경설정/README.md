# go 워크스페이스
- 폴더 안에 항상, bin,pkg,src 폴더가 있어야함
- bin 컴파일링 한 내용 같은게 저장
- pkg 압축된 파일들이 있는곳 -> 어떤 프로그램이 있고, 패키지에서 코드를 모두 가져오게됨 -> 그걸 컴파일링 하고 다른 패키지들이 변경되지 않았다면
아카이브 폴더를 만들고 그것들을 pkg 폴더에 붙임, 그러면 다시 컴파일링 안해도 됨 
- src 네임스페이싱이나 패키지 관리, src 폴더 안의 네임스페이싱은 github.com 같은 도메인이 있음, 그안에 사용자 이름이 있고, 프로젝트 폴더 또는 리포지터리가 있음 -> 네임스페이싱

# go 패키지 받는 방법
- go get github.com/pborman/uuid(패키지 주소)
- https://pkg.go.dev/ -> 패키지 검색

# go 환경변수
GOPATH -> 나의 워크스페이스를 가리킴
GOROOT -> 데이터 설치물을 가리킴 (golang.org)에서 다운로드 한것 

# go모듈생성
- go mod init 모듈이름(네임스페이스로 작성)
- ex) go mod init example.com/test
    - go mod init github.com/

- go get -d github.com/GoesToEleven/go-programming
