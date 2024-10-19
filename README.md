# Misc Cheatsheet

이 레포는 다음과 같은 내용을 포함하고 있습니다.

- 개발과 연구 경험을 배풀고자 만든 레포
- 주니어분들에게 추천하고 싶은 자료들
- 터미널을 사랑하는 사용자들에게

## Linux 

### [Server](linux/server.md)

- 서버 간 파일 전송하기 (`scp`)
- 외부 localhost 접속하기 (`ngrok`)
- 서버 password 변경하기 (`passwd`)
- remote server의 port를 localhost에서 사용하기(`ssh -L` or `ssh -R`)
- 서버의 GUI를 로컬에서 사용하기 (`ssh -X` or `ssh -Y`)
- 서버 ssh-key로 password없이 접속하기 (`ssh-keygen`)
- ssh config 파일 설정으로 간단하게 접속하기 (`~./ssh/config`)

### [GPU](linux/gpu.md)

- 사용 GPU 지정 Python (`CUDA_VISIBLE_DEVICES`)
- CUDA 버전 확인하기 (`nvcc`)
- GPU 사용량 확인하기 (`nvidia-smi`)
- GPU 사용량 확인하기 2 (`nvtop`)
- GPU 사용량 확인하기 3 (`nvitop`)

### [Util](linux/util.md)

- 노트북을 덮거나 시간이 지나도 꺼지지 않게 (`caffeinate`)
- 파일 개수를 알고 싶다면? (`ls -l | grep ^- | wc -l`)
- 디스크의 남은 용량을 알고 싶다면 (`df -h`)
- Syntax Highlight와 함께 cat을 쓰고 싶다면 (`bat`)
- iterm에서 new tab을 만들 때 directory를 유지하고 싶다면?
- 심볼릭 링크 사용하여 바로가기 만들기(`ln -s`)
- pip로 설치 시, 필요없는 output을 보지 않으려면? (`pip install`의 `-q`, `-qq`, `-qqq`)
- tmux에서 마우스 사용하기(`set -g mouse on`)
- json 파일 이쁘게 보기 (`jq`)
- 폰트 추천 (`D2 Coding`)

### Advanced Utils

- [fig](https://github.com/withfig/autocomplete) : 터미널 내부 고급 자동 완성. 미쳐버린 퀄리티...
- [say](https://developer.apple.com/library/archive/documentation/UserExperience/Conceptual/SpeechSynthesisProgrammingGuide/FineTuning/FineTuning.html) : MacOS 전용 TTS 커맨드

### [Vim](linux/vim.md)

- **[vimrc 통합본](linux/.vimrc)**
- (vimrc) 문서 형식 파악 및 문법 하이라이트(`syntax on`, `filetype indent plugin on`)
- (vimrc) 검색, 괄호 등 정보 하이라이트(`hlsearch`, `ruler`, `showmatch`)
- (vimrc) Python 문서 작성에 편리한 모드(종류별 tab 사이즈, `autoindent`)
- (vimrc) 라인 번호 표기(`nu` or `number`)
- (vimrc) 모드별 커서 모양 변경
- vim에서 여러 줄 주석 처리 (`norm i#`, `norm 1x`)
- vim에서 sudo로 저장하기 (`w sudo! tee %`)

### [Git/Github](/linux/github.md)

- Github Profile Badge List : 깃헙을 다양하게 꾸며봅시다.
- 브랜치를 만들면서 바로 체크아웃하려면 (`git checkout -b`)
- 커밋 날짜 바꾸기 (`git commit --amend --no-edit --date`)
- 한글 에러 방지(`core.precomposeunicodem`, `core.quotepath`) 

## Data Science

### Computer Vision

- [albumtations](https://github.com/albumentations-team/albumentations) : Image data augmentation library
- [ttach](https://github.com/qubvel/ttach) : Image Test Time Augmentation with PyTorch
- [timm](https://github.com/rwightman/pytorch-image-models) : Pytorch pre-trained SOTA image models
- [smp](https://github.com/qubvel/segmentation_models.pytorch) : Pytorch pre-trained SOTA image segmentation models

### Prototype

- [Streamlit](https://github.com/streamlit/streamlit) : ML Model을 Web-based GUI로 쉽게 보여주는 오픈소스
- [Gradio](https://github.com/gradio-app/gradio) : ML Model을 Web-based GUI로 쉽게 보여주는 오픈소스

### Tools

- [Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html) : Jupyter Notebook 상위 호환
- [Weights & Biases](https://wandb.ai/) : tensorboard보다 편리한 웹 대시보드

### ETC

- [watermark](https://github.com/rasbt/watermark) : Jupyter에서 라이브러리 버전 명시 익스텐션
- [holidays](https://github.com/dr-prodigy/python-holidays) : 공휴일 구하기. 시계열 데이터에서 유용하게 활용 가능
- [pprint](https://docs.python.org/ko/3/library/pprint.html) : 이쁜 출력을 위한 내장 라이브러리

## Web

### [Flask](web/flask.md)

- Flask에 캐시가 쌓여 새로고침이 안된다면?

### Library & Service

- [Vercel](https://vercel.com/) : 쉬운 배포 서비스

- CSS/Styles
  - [Tailwind UI](https://tailwindui.com/) : 유틸리티 CSS Framework 
  - [Headless UI](https://headlessui.dev/) : Tailwind UI와 함께 사용할 수 있는 UI Components
  - [Chakra UI](https://chakra-ui.com/) : 사용하기 좋은 프레임워크 (추천)
  - [Chakra Templates](https://chakra-templates.dev/) : Chakra로 만든 여러 컴포넌트 제공 
- react
  - [Reactour](https://github.com/elrumordelaluz/reactour) : react에서 onboarding을 도와주는 패키지
  - [react-i18next](https://github.com/i18next/react-i18next) : react 다국어처리 패키지

### Data Visualization(JS)

- [D3](https://d3js.org/) : 하나씩 커스텀하고 싶은 사용자라면 d3
- [Plotly](https://plotly.com/) : 파이썬으로도 사용가능
- [Recharts](https://recharts.org/)
- [Chart.js](https://www.chartjs.org/)
- [Highchart](https://www.highcharts.com/)

## Tool

### Website

- 오픈소스
  - [Codepen](https://codepen.io/) : html/css/js 코드 스니펫 공유 사이트. 다른 사람들을 통해 테크닉을 습득하기도 좋음
- 문서 작업
  - [Thesaurus.com](https://www.thesaurus.com/) : 유의어 사전
  - [Grammarly](https://app.grammarly.com/) : 문법 체크
  - [맞춤법 검사](http://speller.cs.pusan.ac.kr/) : 어떤 문서든 제발...한 번 이상 돌려보길.
- 디자인 작업
  - [flaticon](https://www.flaticon.com/) : 저작권 free 아이콘
  - [Unsplash](https://unsplash.com/) : 저작권 free 이미지
  - [dafont.com](https://www.dafont.com/) : 저작권 free 영어 폰트
  - [carbon](https://carbon.now.sh/) : 코드 공유 이쁘게 만들어주는 사이트
  - [2 Color Combinations](https://2colors.colorion.co/) : 시각화/UI에서 2색 조합을 살펴볼 때 유용한 사이트
- 트렌드
  - [GeekNews](https://news.hada.io/) : 최신 개발/기술/스타트업 뉴스 팔로우업에 좋은 서비스
  - [Product Hunt](https://www.producthunt.com/) : 스타트업의 각자 서비스 공유 플랫폼. 여러 최신 SaaS 등을 살펴볼 수 있음
  - [Disquiet](https://disquiet.io/) : 메이커를 연결해주는 플랫폼. Product Hunt와 유사하게 활용 가능.
- ETC
  - [Ghost](https://ghost.org/) : 깃헙 블로그도 싫고, 티스토리도 싫다면? 유료 블로그 플랫폼
  - [StackShare](https://stackshare.io/) : 기술스택공유 템플릿 사이트
  - 
### Note Taking

- [Notion](https://www.notion.so/) : 이제는 국룰이 되어버린 노트툴
  - [oopy](https://www.oopy.io/) : 노션 페이지를 웹사이트로 만들어주는 서비스
- [Obsidian](https://obsidian.md/) : Roam과 비슷한 기능의 도구
- [Craft](https://www.craft.do/) : Notion과 유사한 툴. MacOS에서 사용하며 더 깔끔한 느낌.
- [Bear](https://bear.app/) : 가벼운 마크다운 툴
- [Roam Research](https://roamresearch.com/) : 그래프 형식으로 마크다운 노트를 정리할 수 있는 도구

### VSCode Extension

- [VSCode Setting Github 계정으로 연동하기](https://code.visualstudio.com/docs/editor/settings-sync)
- [GitLens](https://github.com/Axosoft/vscode-gitlens) : Vscode에서 깃 기록을 앞/뒤로 확인할 수 있는 도구

### Chrome Extension

- [Arxive](https://chrome.google.com/webstore/detail/arxive/hkoblclipggkhhbllgefhnbjdcajmelh/related?hl=ko) : Arxiv 논문 제목을 연도가 아닌 제목-저자 형식으로 바꿔주는 툴
- [Google Scholar Button](https://chrome.google.com/webstore/detail/google-scholar-button/ldipcbpaocekfooobnbcddclnhejkcpn?hl=en) : google scholar 검색을 extension 상에서 할 수 있음.

### Application

- [Todoist](https://todoist.com/) : 투두리스트 관리 툴 - 사용성이 좋음
- [TickTick](https://ticktick.com/) : 투두리스트 관리 툴 - 기능이 많음
- [Mathpix Snip](https://mathpix.com/) : 수식 스크린샷을 LaTex으로 바꿔주는 툴
- [1password](https://1password.com/) : 패스워드 관리 툴
- [Havitica](https://habitica.com/) : 게이미피케이션을 활용한 루틴 관리 툴 

## Articles & Repo

- Articles
  - [오욱환, 학문을 직업으로 삼으려는 젊은 학자들을 위하여](http://home.ewha.ac.kr/~oookwhan/essay/essay2-toyoung.htm) : 대학원생에게 추천하는 글
  - [이직초보 어느 개발자의 이력서 만들기](https://techblog.woowahan.com/2531/) : 처음 CV를 작성하는 분들에게 추천하는 글
  - [subicura님 블로그 : 본격 macOS에 개발 환경 구축하기](https://subicura.com/2017/11/22/mac-os-development-environment-setup.html) : 맥 초기 세팅 가이드라인
- Repos
  - [Modern Unix](https://github.com/ibraheemdev/modern-unix) : 짱짱 멋진 command 명령어 모음
  - [awesome-devteam](https://github.com/leehosung/awesome-devteam) : 좋은 개발팀을 만드는데 도움이 되는 자료 (국문!)
- Youtube & Videos
  - [Ali Abdaal](https://www.youtube.com/channel/UCoOae5nYA7VqaXzerajD0lg) : 생산성 관련 유튜브 채널
  - [How great leaders inspire action](https://www.ted.com/talks/simon_sinek_how_great_leaders_inspire_action/up-next?language=en) : Golden Circle의 창시자 사이먼 시넥의 TED 발표. 왜?를 먼저 생각해야 하는 이유.
- Books
  - [타이탄의 도구들(팀 페리스 저)](https://shopping.interpark.com/product/productInfo.do?prdNo=8577355413) : 성장하고 싶은 이들을 위해.
  - [소프트 스킬(존 손메즈 저), 길벗](http://www.yes24.com/Product/Goods/23161141) : 개발자에게 필요한 역량에 대한 다양한 조언을 줄 수 있는 책입니다.
  - [초생산성(마이클 하야트 저), 로크미디어](http://www.kyobobook.co.kr/product/detailViewKor.laf?mallGb=KOR&ejkGb=KOR&barcode=9791135465512) : 생산성에 대해 생각해보고, 본인의 삶을 더 자유롭게 만드는 책

</br>

### This repository was cloned by https://github.com/subinium/Misc-Cheatsheet
