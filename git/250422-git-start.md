## Today I learned
- what is the git?
	- Linus Torvals가 화나서 1주일 만에 만든 최고의 버전관리 도구
	- 장점 : 분산형 저장소, 비선형적 개발 가능
- GitHub Profile README Generator : https://rahuldkjain.github.io/gh-profile-readme-generator/
	- GitHub 사용자 프로필Repository : YeonkyungKang/YeonkyungKang
	- repository를 생성하면 GiHub 프로필 상단에 README 내용을 자동으로 노출할 수 있음.
    - README.md 파일을 작성하며, 그 내용이 GiHub 프로필 상단에 표시된다. 마크다운으로 작성함
- 저장소 운용할 때 잊으면 안되는 것
	- README.md
	- .gitignore : https://www.toptal.com/developers/gitignore/
	- 
- Git 버전관리 흐름 : working Directory -> Staging Area -> Local repository -> Remote Repository
  ( - -> git add -> git commit -> git push , 상태 보기:git status )
- Git branch 관리
	- git branch : 작업 단위[공간] 분리
	- git switch : branch 전환 
	- git merge : branch 병합 (기능 통합 및 최종 반영)
- Git branch 작업 순서
	- 1. branch 생성: git branch [new branch name]
	- 2. branch 이동: git swich [branch name]
	- 3. 기능 구현 완료 -> main branch 전환 -> 병합: git swich main -> git merge [branch name/file_name]
	- 4. 작업 branch 반영 후 branch 삭제: git branch -d [branch name]
- Git : 시간 + 공간
| 요소         | 개념                           | Git 구성 요소                  |
|-----------|----------------------------------|--------------------------------|
|시간(Time) | 변화를 기록하는 연속성              | `commit`, `log`, `revert`      |
|공간(Space)| 독립적이고 병렬적인 작업 공간       | `branch`, `switch`, `merge`    |
|시간+공간  | 협업·복원      | 브랜치 기반 커밋 히스토리 관리 |
- Conventional Commits :https://www.conventionalcommits.org/ko/v1.0.0/
	- <타입>(범위):<설명>
 	- feat : 기능 개발 관련 ex)feat : Create main.py 
    - fix : 오류 개선 혹은 버그 패치 ex)fix(form): Fix required field bug
	- docs: 문서화 작업	  ex)docs: Correct spelling of CHANGELOG
	- test : test 관련		
	- conf: 환경설정 관련 
	- build : 빌드 작업 관련
	- ci : Continuous Integration 관련
	- chore: 패키지 매니저, 스크립트 등	 ex)chore!: Drop support for Node 6
	- style: 코드 포매팅 관
