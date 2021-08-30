# code-with
----------------------------------------------------------------------
<codeWith 프로젝트를 진행하며 겪은 어려움, 해결방법 등 정리>

1. 학습을 진행하기 위해 코드 편집기가 필요하고, 결과를 바로 볼 수 있도록 해야하는데 이를 어떻게 해결하였나?
:  코드 편집기를 구현하기 위해선 신경쓸것들이 매우 많다. 줄 간격, 들여쓰기, 사용자의 편의를 위한 색상 구별, 사용자가 입력한 코드를 문자 그대로가 아닌, 코드로 인식될수 있도록 처리하는 작업, 사용자가 입력한 코드를 실시간으로 실행결과를 보여주도록 하는 작업, html/css/js별로 편집기 분리 등등을 다 구현하기에는 시간적으로도, 내 능력상으로도 매우 힘든 작업이 될 터였다. 일일히 구현하기 보다는 오픈소스/툴을 이용하여 해결해야겠다고 마음먹고, 구글링을 한 결과 codepen이라는 툴을 알게 되었고 이를 codeWith 홈페이지에 embed하는 방식으로 해결하였다. 그대로 갖다 썼다기 보다는, 코드윗 홈페이지의 ui와 어울리도록 그리고 생각해놓은 커리큘럼에 걸맞도록 수정하여 이용자가 편하게 코드를 입력하도록 하였다. 예를들어, 사용자가 css 달력 만들기 코스를 진행한다고 하면 그에 필요한 달력 html 코드가 미리 들어가있게끔 하는 식이다.  

2. 처음으로 프레임워크를 사용해보면서 겪은 가장 큰 어려움은?
: 무엇보다 프레임워크를 처음 시도한다는 압박감이 컸다. 제출까지의 기간이 그리 넉넉한것도 아닌데 무언가를 새로 배워서 바로 응용해야 한다는 부담이 있었다. vue가 react등 다른 프레임워크에 비해 쉬운편이라고 들어서 선택하긴 했지만, vue의 문법, 라이프사이클, 라우트, 컴포넌트 간의 통신 등을 이해하는 데에는 시간이 필요했다. 유튜브 강의를 찾아 시청하고, 무작정 구글링하고, 책도 봐가며 최대한 많이 이해하려고 노력한것 같다. 더 공부해서 다음 프로젝트떄는 vue의 장점을 최대한으로 살려서 더 잘 이용해보고 싶다는 생각이 든다.   

3.  코딩하다가 어느 부분에서 막혔는가?
: 이전에도 간단한 웹페이지 제작 프로젝트를 진행해본적이 있긴 하지만, 사이트 배포단계까지 가본것은 이번이 처음인지라 통신을 하는 부분에서 처음에 막막감을 느꼈다. get, post 등 많이 들어보기는 했지만 언제 어느 상황에서 데이터를 불러오고 보내야 하는지에 대한 타이밍이라던지, 무엇을 어떻게 보내야 하는지 등 초반에 생각 정리가 잘 안됐던것같다. 내린 결론은, 해보다보면 어떤 식으로 돌아가는지 감이 잡힌다는 것이다. 함께 프로젝트를 진행했던 분들이 잘 해주셔서 다행히 통신이 원활하게 될 수 있었던 것 같다. 데이터가 잘 불러와 보여지는 순간 신이 나기도 했다. 

4. 코드윗이라는 웹페이지를 만들면서 특히 신경쓴 부분이 있다면?
: 완전한 입문자들이 맛보기로 프론트엔드 코딩을 배울 수 있도록 하는, 초심자들을 위한 코딩학습 사이트가 컨셉이므로 딱딱하지 않아 보이면서 최대한 완성도가 있어보이는 ui를 만들기 위해 힘썼다. 기능들이 화려하게 이것저것 있지 않은 대신 사소한 디테일까지도 신경쓰며 웹 설계를 했던것같다. 직관적이면서 편리한 기능 이용이 가능하도록 수정에 수정을 거듭하여 완성도를 높이고자 하였다. 글자의 크기, 배치, 간격 등 세부적인 조정들을 신경써서 했다. 또한, 기본이라고도 볼 수 있는 로그인 기능을 잘 녹여내기 위하여 학습 페이지 내에서 로그인/로그아웃 또한 가능하게 했고, 로그아웃 했을 시의 차별점들까지 고려하여 설계하였다(로그아웃하면 튜토리얼 단계까지 이용이 가능하다). 또한 vue의 특징으로 컴포넌트 단위로 화면을 구획하여 재사용이 용이하다는 점이 있는데, 이 장점을 잘 살리고자 했던것 같다. 

5. 프로젝트를 진행하면서 느낀점(무엇을 배웠다거나, 다음부터는 어떤것을 어떤식으로 해야겠다고 느꼈다던가)
: 이전에는 css를 다소 마구잡이로 사용한 감이 없지않아 있었는데, 이번에는 좀더 체계적이고 일관된 방식으로 사용하는 감을 익히게 되었다. 예를들어 어떤 부분에서는 flex 기능을 이용하는것이 좋고, 어떤 부분은 position으로 배치해야 하는지와 같은 부분들을 많이 배웠다. 그리고 사소한 변경인것처럼 보여도 다른 요소에 영향을 줄 수 있다는 점을 명심하게 되었다. 후반부에 폰트를 전반적으로 바꿨는데, 폰트때문에 비밀번호 입력 란에 입력하면 보여져야 할 동그라미가 보이지 않게 되는것이 아닌가. 정말이지, 프론트엔드는 꼼꼼한 점검이 정말 많이 필요한것 같다고 느꼈다. 그리고, 개발 언어에 대한 공부를 더 많이 해야겠다고 느꼈다. 나중에 돌아보면 간단한 코드로 구현이 가능한 부분들도, 그때 당시에는 뭐가 뭔지 잘 몰라서 한참 헤맸다. 자바스크립트 공부를 좀더 했었더라면 불필요하게 삽질하던 시간을 줄일 수 있지 않았을까 하는 아쉬움이 들기도 하다. 물론 아쉬운 부분들도 많았지만, 무엇보다 이번 프로젝트를 통해 많이 배워갈 수 있었어서 정말 후회하지 않는다. 다음 프로젝트를 진행할 때엔 더 발전되어 있을 나의 모습이 기대되기도 하다. 




## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
