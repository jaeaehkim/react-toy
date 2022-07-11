# react-toy

## 프로젝트 시작
- npx create-react-app tic-tac-toe
    - node_modules, public, src, package.json 기본 세팅을 자동으로 해줌
    - package.json
        - react/react-dom > 웹개발을 위한 라이브러리
        - react-scripts > 배포를 위한 라이브러리
        - @testing > 테스트를 도와주는 라이브러리
        - scripts
            - npm start : 개발모드로 로컬에서 띄어주는
            - npm run build : 개발 작업을 끝낸 후 배포할 준비, 프로덕션모드 > 소스파일들을 최적화시켜 컴파일 (build폴더가 생성됨)
                - build라는 폴더를 파일서버로 이용
            - npx serve -s build : build폴더를 활용해서 serving
                - 개발모드 vs 프로덕션모드 차이 : 코드 최적화 여부
            - npm test : testing 환경이 이미 구성되어 있고 그걸 통해 testing
            - npm eject : 환경설정을 custom하게 하기 위해선 creat-react-app에서 꺼내서 쓰는 경우 -> 실무에서 잘 활용하진 않음. 관리하기 어려움.
                - 실제로 eject하는 경우에 package.json > dependencies 의 여러 key들이 생성됨. react-scripts에서 관리되던 것들이 다 pop up
                - jest 폴더가 생기고 이런 것들을 전부 customizing 가능
