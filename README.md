# [ STUDY - D3.js ]

## 20140725

### 1. D3.js
#### 1. 무엇을 위한 라이브러리인가?
D3는 데이터 중심의 문서(Data-Driven Documents)라는 이름의 약어.
데이터 시각화 제작을 위한 js 라이브러리로 영국 개발자 mike bostock이 2011년에 개발. 
BSD 라이선스 배포이므로, 비용 없이 영리/비영리 목적 상관없이 코드 사용/수정 가능.

#### 2. 어떻게 작동하는가?
1. 데이터를 로드한다 (loading)
2. Html element를 만들어 데이터를 엮는다 (binding)
3. Element에 엮인 개별 데이터를 토대로 element를 변화시킨다. (transforming)
4. 사용자 입력에 따른 interaction을 수행한다. (transitioning)

#### 3. 사용상 이슈
SVG는 ie8 이하 미지원.

#### 4. 샘플
http://christophermanning.org/projects/building-cubic-hamiltonian-graphs-from-lcf-notation/ 
http://www.jasondavies.com/maps/transition/ 
http://www.nytimes.com/interactive/2012/02/13/us/politics/2013-budget-proposal-graphic.html 
http://bl.ocks.org/mbostock/1044242 
http://bl.ocks.org/mbostock/4339083 

#### 5. D3의 대안들
https://datawrapper.de/ 
http://www.flotcharts.org/ 
http://g.raphaeljs.com/ - IE6 포함 지원.
http://www.highcharts.com/ - 비영리 목적이라면 무료. 
http://www.jqplot.com/ - jQuery 차트 플러그인. Ie7 이상 지원.
http://benpickles.github.io/peity/ - 아주 작고 단순한 미니 차트
http://yuilibrary.com/yui/docs/charts/ - Yahoo 가 만든 차트 모듈.
http://arborjs.org/ - canvas 사용.
http://sigmajs.org/ - canvas 사용.
http://helloworld.naver.com/helloworld/651829 - Naver 에서 개발한 Nwagon

#### 6. D3 유틸
1. 라이브코딩 테스트툴 : http://tributary.io/ 
2. 한글화 문서 : https://github.com/zziuni/d3/wiki
3. 한글화 API : https://github.com/zziuni/d3/wiki/API-Reference


### 2. D3 문법 맛보기
1. 기본 문법 / 체인 문법
파일 : sample_grammar.html

2. Load CSV Data 
파일 : sample_loadData.html
grunt connect 등으로 local server 실행 후, 접속하여 테스트.

3. Data bind 
파일 : sample_bindData.html

4. div element chart 그리기
파일 : sample_divChart.html

### 3. SVG 문법 맛보기
1. SVG는 무엇인가?
참고) http://www.w3schools.com/svg/ 
Scalable Vector Graphics의 줄임말.
IE8 이하를 제외한 대부분의 브라우저가 지원( http://caniuse.com/#search=svg )

2. SVG 선언
<svg width=”500” height=”50”></svg>
단위는 px 이 기본이며,
canvas와 비슷함. ( <canvas id=”myCanvas” width=”500” height=”50”></canvas> )

3. SVG 도형 그리기
SVG 도형의 종류는 rect, circle, ellipse, line, polygon, polyline, path, text 
파일 : sample_svg.html

### 4. D3로 SVG 그리기

1. SVG chart그리기
파일 : sample_svgChart.html

2. SVG chart에 Label 더하기
파일 : sample_svgChartAddLabel.html

3. SVG chart에 mouse event 더하기
파일 : sample_svgChartMouseEvent.html