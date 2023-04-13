# FIRST

## 🐱‍🐉브랜치가 여러 개일 때 어떻게 업로드 할까요?
먼저, clone부터 시작해봅시당
git clone [repository 주소]를 git bash나 vsc 터미널에 입력해주시면 자동으로 git 저장소가 로컬 환경에 생성됩니다!
해당 폴더로 이동한 뒤,
develop 브랜치를 생성해줍니다.
먼저 main 브랜치에서 파일을 생성해줍니다!
그 다음 add commit push를 진행해주세요~!
그럼 현재 main에는 파일들이 있지만 develop에는 아무 파일도 없습니다!
develop에 파일을 땡겨줄까요?
develop으로 checkout 해줍니다.
그 다음 git pull origin main을 진행해주면 develop에 main의 파일들이 똑같이 생성됩니다!
이때 working directory에는 아무 수정 사항이 없으므로 git add . 가 실행되지 않습니다!
따라서 우리는 한 파일을 수정해 준 뒤, 다시 add commit push를 진행해줍니다!
그러면 원격 저장소인 github 페이지에도 develop브랜치와 파일들이 생성되어 있어요!
예~!

## 🤷‍♂️순서 정리
1. git clone
2. 브랜치 생성(보통은 공통 파일을 만들어 준 뒤 각자 브랜치 생성)
3. main 브랜치에서 작업 및 add commit push
4. develop 브랜치에서 수정 및 add commit push
5. featureA 브랜치에서 수정 및 add commit push
6. 다른 브랜치에서 파일들을 불러오려면? => git pull origin develop(featureA 브랜치에 checkout 되어있다고 가정했을때)
7. 완성 후 commits를 확인하면 pull이 merge와 똑같이 사용되는 것을 볼 수 있습니다~! 하지만 완전 똑같은건 아니예용~!
