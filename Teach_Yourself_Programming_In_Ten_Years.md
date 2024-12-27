# 10년 안에 프로그래밍 독학하기

## 왜 다들 그렇게 서두르는 걸까요?

어떤 서점에 들어가 보아도, _《24시간 만에 Java 독학하기》_ 와 같이 C, SQL, Ruby, 알고리즘 등을 며칠 혹은 몇 시간 만에 배울 수 있다고 주장하는 무수한 책들을 볼 수 있습니다. 아마존에서 [[title: teach, yourself, hours, since: 2000]](http://www.amazon.com/gp/search/ref=sr_adv_b/?search-alias=stripbooks&unfiltered=1&field-keywords=&field-author=&field-title=teach+yourself+hours&field-isbn=&field-publisher=&node=&field-p_n_condition-type=&field-feature_browse-bin=&field-subject=&field-language=&field-dateop=After&field-datemod=&field-dateyear=2000&sort=relevanceexprank&Adv-Srch-Books-Submit.x=16&Adv-Srch-Books-Submit.y=5) 라는 고급 검색을 하면, 그런 책이 512권이나 나옵니다. 그 중 상위 10권 중 9권은 프로그래밍 관련 책입니다 (나머지 한 권은 회계에 대한 책입니다). "teach yourself"를 "learn"으로, "hours"를 "days"로 바꿔도 비슷한 결과를 얻을 수 있습니다.

결론은 사람들이 굉장히 급하게 프로그래밍을 배우려고 하거나, 아니면 프로그래밍이 다른 어떤 것보다도 배우기 훨씬 쉬운 것처럼 보인다는 것입니다. Felleisen _et al._ 는 책 [《How to Design Programs》](https://www.amazon.com/How-Design-Programs-Introduction-Programming/dp/0262062186)<sup>\*</sup>에서 "나쁜 프로그래밍은 쉽다. *바보*들도 _21일 만에_ 배울 수 있다, 심지어 그들이 *얼간이*라도."라고 말하며 이런 추세를 풍자적으로 언급합니다. Abstruse Goose 만화도 이에 대해 [_자신만의 관점_](https://web.archive.org/web/20150417191951/http://abstrusegoose.com/249)을 표현했습니다.<sup>\*\*</sup>

> \*: [원본 링크](http://www.ccs.neu.edu/home/matthias/HtDP2e/index.html) 접속이 불가하여 아마존 책 링크로 대체합니다. (역주)
>
> \*\*: 원본 [The Abstruse Goose - How to Teach Yourself Programming](http://abstrusegoose.com/249) 페이지가 서비스 종료되어 web archive 링크로 대체합니다. (역주)

다음은 [《24시간 만에 C++ 독학하기》](http://www.amazon.com/Sams-Teach-Yourself-Hours-5th/dp/0672333317/ref=sr_1_6?s=books&ie=UTF8&qid=1412708443&sr=1-6&keywords=learn+c%2B%2B+days)라는 제목이 의미할 수 있는 바를 분석해 보겠습니다:

- **독학하기(Teach Yourself):**  
  24시간 안에는 여러 중요한 프로그램을 작성하고, 성공과 실패를 통해 배우는 것이 불가능합니다. 또한, 경험 많은 프로그래머와 함께 일하면서 C++ 환경에서의 삶이 어떤지 이해할 시간도 없습니다. 요컨대, 24시간 안에는 깊은 이해를 얻을 시간이 없습니다. 따라서 이런 책들은 깊이 있는 이해가 아니라 단순히 피상적인 친숙함을 제공한다고 봐야 합니다. 알렉산더 포프(Alexander Pope)는 이렇게 말했습니다. "조금 배운 것은 위험하다(A little learning is a dangerous thing)."

- **C++:**  
  만약 이미 다른 프로그래밍 언어를 알고 있다면, 24시간 동안 C++의 문법 일부를 배울 수는 있을 것입니다. 그러나 그 언어를 어떻게 사용하는지에 대해서는 거의 배울 수 없습니다. 예를 들어, 베이직(Basic) 언어를 아는 사람이 C++ 문법을 사용하여 베이직 스타일의 프로그램을 작성하는 법은 배울 수 있겠지만, C++의 장점과 단점이 무엇인지 배우지는 못할 것입니다. 그렇다면 이런 책의 목적은 무엇일까요? [앨런 퍼리스(Alan Perlis)](https://www.cs.yale.edu/homes/perlis-alan/quotes.html)<sup>\*</sup>는 이렇게 말했습니다. "프로그래밍에 대한 사고 방식을 변화시키지 않는 언어는 배울 가치가 없다." 한 가지 가능성은, C++의 작은 부분(혹은 JavaScript나 Processing 같은 다른 언어)을 배우는 이유가 특정 작업을 수행하기 위해 기존 도구들 활용해야 하기 때문일 수 있습니다. 그러나 이 경우에도 그것은 프로그래밍을 배우는 것이 아니라 단지 그 작업을 수행하는 방법을 배우는 것에 지나지 않습니다.

  > \*: [원본 링크](http://www-pu.informatik.uni-tuebingen.de/users/klaeren/epigrams.html) 접속이 불가하여 대체합니다. (역주)

- **24시간 안에:**  
  불행히도, 다음 섹션에서 설명하겠지만 이는 충분하지 않습니다.

## 10년 안에 프로그래밍 독학하기

연구자들([Bloom (1985)](http://www.amazon.com/exec/obidos/ASIN/034531509X/), [Bryan & Harter (1899)](#참고문헌), [Hayes (1989)](http://www.amazon.com/exec/obidos/ASIN/0805803092), [Simmon & Chase (1973)](#참고문헌))에 따르면 체스, 음악 작곡, 전신 운용, 그림 그리기, 피아노 연주, 수영, 테니스, 신경심리학 및 토폴로지 연구 등 다양한 분야에서 전문성을 갖추기까지 약 10년이 걸린다고 합니다. 그 핵심은 "**_의도적인_** 연습"(deliberative practice)에 있습니다. 단순히 반복하는 것이 아니라, 자신의 현재 능력을 약간 넘어서는 도전을 하고, 그것을 시도하며, 수행 과정을 분석하고, 실행 중이거나 실행 후에 실수를 수정하는 것입니다. 그리고 이를 반복하고 또 반복하는 것입니다. 진정한 지름길은 존재하지 않는 것처럼 보입니다. 어린 시절부터 음악 신동으로 불린 모차르트조차 4살에 처음 음악적 재능을 보였지만, 세계적인 수준의 음악을 만들기까지 13년이 더 걸렸습니다. 다른 예로, 비틀즈는 1964년 에드 설리번 쇼에 출연하며 연이어 1위 히트곡을 내놓으며 갑자기 등장한 것처럼 보였지만, 사실 그들은 1957년부터 리버풀과 함부르크의 작은 클럽에서 공연해 왔습니다. 초기에는 대중적인 인기를 얻었지만, 첫 번째 비평적 성공작인 *Sgt. Peppers*는 1967년에야 출시되었습니다.

[말콤 글래드웰(Malcolm Gladwell)](https://www.amazon.com/Outliers-Story-Success-Malcolm-Gladwell/dp/0316017922)은 이 개념을 대중화했지만, 그는 10년이 아닌 10,000시간에 초점을 맞췄습니다. 앙리 카르티에-브레송(Henri Cartier-Bresson, 1908-2004)은 또 다른 기준을 제시했습니다. "당신의 첫 10,000장의 사진은 최악이다." (디지털 카메라 시대에서는 어떤 사람들은 일주일 만에 이 수치에 도달할 수 있다는 점을 그는 예상하지 못했습니다.)

진정한 전문성은 평생이 걸릴 수도 있습니다. 새뮤얼 존슨(Samuel Johnson, 1709-1784)은 이렇게 말했습니다. "어떤 분야에서든 탁월함은 평생의 노력으로만 얻을 수 있다. 싼 값에 얻을 수 있는 것이 아니다." 또한, 초서(Geoffrey Chaucer, 1340-1400)는 "삶은 너무 짧고, 기술을 배우는 것은 너무 길다"라고 한탄했습니다. 히포크라테스(Hippocrates, 기원전 약 400년)는 "ars longa, vita brevis"라는 표현으로 알려져 있으며, 이는 긴 인용문인 _"Ars longa, vita brevis, occasio praeceps, experimentum periculosum, iudicium difficile"_ 의 일부입니다. 이를 번역하면 "삶은 짧고, 기술은 길며, 기회는 잠깐이고, 실험은 위험하며, 판단은 어렵다"라는 뜻입니다. 물론, 10000이라는 숫자 하나가 모든 것의 정답일 수는 없습니다. 예를 들어, 프로그래밍, 체스, 체커, 음악 연주와 같은 기술을 익히는 데 모두 동일한 시간이 걸린다고 가정하는 것은 비합리적으로 보입니다. 또한, 모든 사람들이 동일한 시간을 필요로 한다고 생각하는 것도 비현실적입니다.

[K. 안데르스 에릭슨(K. Anders Ericsson)](http://www.amazon.com/K.-Anders-Ericsson/e/B000APB8AQ/ref=dp_byline_cont_book_1) 교수는 이렇게 설명합니다. "대부분의 분야에서 가장 뛰어난 사람들도 최고 수준의 성과에 도달하기 위해 얼마나 많은 시간이 필요한지는 놀라울 정도입니다. 10,000시간이라는 숫자는 우리가 이야기하고 있는 것이 주당 10~20시간 동안 몇 년간 연습해야 한다는 점을 보여주는 것에 불과합니다. 심지어 타고난 재능이 있다고 여겨지는 사람들도 최고 수준에 도달하려면 이 정도 시간이 필요합니다."

## 프로그래머가 되고 싶으신가요?

프로그래밍을 잘하게 되는 제 비법들은 아래와 같습니다:

- **프로그래밍에 흥미를 가지세요**. 프로그래밍은 재미있으니까 직접 해 보세요. 이 과정이 충분히 재미있도록 유지하세요. 그래야만 10년/10,000시간이라는 시간을 투자할 수 있습니다.

- **프로그래밍하세요.** 최고의 학습 방식은 [직접 해 보는 것](http://www.engines4ed.org/hyperbook/nodes/NODE-120-pg.html)<sup>\*</sup>입니다. 좀 더 기술적으로 말하자면, "특정 도메인에서 개인의 최대 성과 수준은 단순히 오랜 경험의 결과로 자동으로 도달되지 않으며, 숙련된 개인조차도 개선을 위한 의도적인 노력의 결과로 성과 수준을 높일 수 있다." [(366쪽)](https://mrbartonmaths.com/resourcesnew/8.%20Research/Explicit%20Instruction/Deliberate%20Practice.PDF)<sup>\*\*</sup> 또한, "가장 효과적인 학습은 특정 개인에게 적절한 난이도를 가지고 잘 정의된 과제, 유익한 피드백, 그리고 반복 및 오류 수정의 기회를 필요로 한다." (20-21쪽) 이 관점에서 [**《Cognition in Practice: Mind, Mathematics, and Culture in Everyday Life》**](http://www.amazon.com/exec/obidos/ASIN/0521357349)라는 책은 흥미로운 참고 자료가 될 수 있습니다.

> \*: 원본 링크가 접속 불가한데 해당 자료를 찾을 수 없었습니다. (역주)

> \*\*: [원본 링크](http://www2.umassd.edu/swpi/DesignInCS/expertise.html) 접속이 불가하여 [google scholar](https://scholar.google.com/citations?view_op=view_citation&hl=en&user=Ym0clGUAAAAJ&citation_for_view=Ym0clGUAAAAJ:u-x6o8ySG0sC) 의 링크로 대체합니다.

- **다른 프로그래머들과 대화하고, 다른 프로그램 코드를 읽으세요.** 이는 어떤 책이나 훈련 코스보다도 중요합니다.

- 원한다면, **대학에서 4년(또는 대학원에서 더 많은 시간)을 보내세요.** 이는 자격/학위를 요구하는 몇몇 직업에 접근할 수 있게 해 주고, 이 분야에 대해 깊이 이해할 수 있도록 할 것입니다. 하지만 학교를 좋아하지 않는다면, 어느 정도의 노력을 통해 독학 또는 현장에서 비슷한 경험을 얻을 수 있습니다. 어쨌든 책만으로는 충분하지 않습니다. 에릭 레이먼드(Eric Raymond) 는 그의 저서 _《The New Hacker's Dictionary》_ 에서 "컴퓨터 과학 교육은 누군가를 전문 프로그래머로 만들 수 없다. 이것은 붓과 안료에 대해 공부하는 것이 누군가를 전문 화가로 만들 수 없는 것과 같다."라고 말합니다. 제가 고용했던 최고의 프로그래머 중 한 명은 고등학교 졸업장이 전부였지만, 그는 많은 [훌륭한](http://www.xemacs.org/) [소프트웨어](http://www.mozilla.org/)를 만들어 냈고, [뉴스 그룹](http://groups.google.com/groups?q=alt.fan.jwz&meta=site%3Dgroups)을 운영하며, 스탁옵션으로 [나이트클럽](http://en.wikipedia.org/wiki/DNA_Lounge)을 살 만큼의 돈을 벌었습니다.

- **다른 프로그래머들과 프로젝트를 진행하세요.** 어떤 프로젝트에서는 최고의 프로그래머가 되세요. 또 어떤 프로젝트에서는 최악의 프로그래머가 되세요. 최고의 프로그래머일 때는 프로젝트를 이끄는 능력을 테스트하고, 자신의 비전으로 다른 사람들을 고무시킬 수 있습니다. 최악의 프로그래머일 때는 거장들이 무엇을 하는지 배우고, 그들이 하기 싫어하는 일(그들이 당신에게 맡기는 일)을 배우게 됩니다.

- **다른 프로그래머가 작업한 후의 프로젝트에서 일하세요.** 누군가 다른 사람이 작성한 프로그램을 이해하세요. 원래의 프로그래머가 없는 상태에서 그 프로그램을 이해하고 수정하려면 무엇이 필요한지 보세요. 자신의 프로그램을 유지보수하기 쉽게 설계하려면 어떻게 해야 하는지 고민해 보세요.

- **적어도 6개 이상의 프로그래밍 언어를 배우세요.** 클래스 추상화를 강조하는 언어(Java나 C++), 함수형 추상화를 강조하는 언어(Lisp, ML, Haskell), 구문 추상화를 지원하는 언어(Lisp), 선언적 명세를 지원하는 언어(Prolog나 C++ 템플릿), 병렬성을 강조하는 언어(Clojure나 Go)를 포함하도록 하세요.

- **"컴퓨터 과학"에는 "컴퓨터"가 포함된다는 것을 기억하세요.** 컴퓨터가 명령을 실행하는 데 걸리는 시간, 캐시 미스가 있을 때와 없을 때 메모리에서 단어를 가져오는 시간, 디스크에서 연속된 단어를 읽는 시간, 디스크의 새 위치로 이동하는 데 걸리는 시간을 알아 두세요. (**[정답 보기](#정답)**)

- **언어 표준화 작업에 참여해 보세요.** ANSI C++ 위원회와 같은 공식적인 작업일 수도 있고, 로컬 코딩 스타일의 들여쓰기 수준을 2칸으로 할지 4칸으로 할지 결정하는 것일 수도 있습니다. 어쨌든, 이를 통해 다른 사람들이 언어에서 무엇을 좋아하는지, 그것에 대해 얼마나 깊이 느끼는지, 그리고 어쩌면 왜 그렇게 느끼는지까지 배우게 될 것입니다.

- **언어 표준화 작업에서 가능한 빨리 빠져나올 지혜를 가지세요.**

그 모든 점을 염두에 두고 보면, 책을 읽는 것 만으로 얼마나 멀리 갈 수 있을지 의문입니다. 첫 아이가 태어나기 전, 저는 온갖 _《How To》_ 책을 읽었지만 여전히 아무것도 모르는 초보처럼 느껴졌습니다. 30개월 후, 둘째 아이가 태어날 때가 되었을 때, 다시 책을 읽으며 복습했을까요? 아닙니다. 대신, 저는 제 개인적인 경험에 의존했는데, 이는 전문가들이 쓴 수천 페이지의 글보다 훨씬 더 유용하고 안심이 되었습니다.

프레드 브룩스(Fred Brooks)는 그의 에세이 [《No Silver Bullet》](http://en.wikipedia.org/wiki/No_Silver_Bullet)에서 훌륭한 소프트웨어 디자이너를 발굴하기 위한 세 가지 계획을 제시했습니다:

1. 가능한 한 빨리 최고의 디자이너들 체계적으로 선별합니다.
2. 경력 멘토를 지정하여 후보자들의 발전을 책임지게 하고, 경력 파일을 신중하게 관리합니다.
3. 성장하는 디자이너들이 서로 교류하고 자극을 받을 기회를 제공합니다.

이 계획은 몇몇 사람들이 이미 훌륭한 디자이너가 되기 위한 자질을 가지고 있다고 가정하며, 이 자질을 적절히 끌어내는 것이 과제라는 점에 기초합니다. [앨런 퍼리스(Alan Perlis)](https://www.cs.yale.edu/homes/perlis-alan/quotes.html)<sup>\*</sup>는 이를 더 간결하게 표현했습니다:  
"누구든지 조각을 배우도록 가르칠 수 있다. 미켈란젤로는 조각을 하지 않는 방법을 배워야 했을 것이다. 훌륭한 프로그래머도 마찬가지다." 퍼리스의 말은 위대한 인물들은 훈련을 초월하는 어떤 내적 자질을 가지고 있다는 의미입니다. 하지만 그 자질은 어디에서 오는 것일까요? 이는 타고나는 것일까요? 아니면 부단한 노력으로 개발되는 것일까요? 영화 *라따뚜이*에 등장하는 가상의 셰프 오귀스트 구스토(Auguste Gusteau)는 이렇게 말합니다. "누구나 요리를 할 수 있다. 그러나 두려움 없는 자만이 위대해질 수 있다." 저는 이것을 _'의도적인 연습에 삶의 큰 부분을 바치는 의지'_ 라고 생각합니다. 하지만 어쩌면 **'두려움 없이'** 가 이를 요약하는 한 방법일 수도 있겠습니다 구스토의 비평가인 안톤 이고(Anton Ego)는 이렇게 말합니다: "모두가 위대한 예술가가 될 수 있는 것은 아니지만, 위대한 예술가는 어디에서나 나올 수 있다."

> \*: [1절](#왜-다들-그렇게-서두르는-걸까요) 에서와 같은 링크로 대체했습니다. (역주)

그러니 Java, Ruby, JavaScript, PHP 책을 사세요. 아마 어느 정도 유용하게 사용할 수 있을 것입니다. 그러나 24시간이나 21일 안에 당신의 삶을 바꾸거나 프로그래머로서의 실제 전문성을 획득할 수는 없습니다. 그렇다면 24개월 동안 꾸준히 노력하며 개선하는 것은 어떨까요?

이제야 좀 진전이 보이네요...

## 참고문헌

- Bloom, Benjamin (ed.) Developing Talent in Young People, Ballantine, 1985.

- Brooks, Fred, No Silver Bullets, IEEE Computer, vol. 20, no. 4, 1987, p. 10-19.

- Bryan, W.L. & Harter, N. "Studies on the telegraphic language: The acquisition of a hierarchy of habits. Psychology Review, 1899, 8, 345-375

- Hayes, John R., Complete Problem Solver Lawrence Erlbaum, 1989.

- Chase, William G. & Simon, Herbert A. "Perception in Chess" Cognitive Psychology, 1973, 4, 55-81.

- Lave, Jean, Cognition in Practice: Mind, Mathematics, and Culture in Everyday Life, Cambridge University Press, 1988.

## 정답

일반적인 PC에서 다양한 작업에 소요되는 대략적인 시간:

| 작업                                       |                            시간 |
| :----------------------------------------- | ------------------------------: |
| 일반적인 명령 실행                         |   1/1,000,000,000 초 = 1 나노초 |
| L1 캐시 메모리에서 데이터 가져오기         |                      0.5 나노초 |
| branch 예측 실패                           |                        5 나노초 |
| L2 캐시 메모리에서 데이터 가져오기         |                        7 나노초 |
| Mutex 잠금/해제                            |                       25 나노초 |
| 주 메모리에서 데이터 가져오기              |                      100 나노초 |
| 1Gbps 네트워크로 2K 바이트 전송            |                   20,000 나노초 |
| 메모리에서 1MB를 순차적으로 읽기           |                  250,000 나노초 |
| 디스크의 새 위치에서 데이터 가져오기(탐색) |                8,000,000 나노초 |
| 디스크에서 1MB를 순차적으로 읽기           |               20,000,000 나노초 |
| 미국에서 유럽으로 패킷 전송 후 응답 받기   | 150 밀리초 = 150,000,000 나노초 |

## 부록: 프로그래밍 언어 선택

많은 사람들이 처음 어떤 프로그래밍 언어를 배워야 하는지 물어옵니다. 이에 대한 정답은 없지만, 다음 사항을 고려해 보세요:

- _친구를 활용하세요._  
  "Windows, Unix, 아니면 Mac 중에 어떤 운영체제를 사용해야 하나요?" 라는 질문을 받으면, 저는 보통 이렇게 대답합니다: "친구들이 사용하는 것을 고르세요." 친구들에게 배울 수 있는 이점은 운영체제나 프로그래밍 언어 간의 본질적인 차이를 상쇄해 줄 것입니다. 또한, 미래의 친구들, 즉 앞으로 프로그래밍을 계속한다면 속하게 될 프로그래머 커뮤니티도 고려하세요. 선택한 언어가 큰 성장을 이루고 있는 커뮤니티를 가지고 있나요, 아니면 쇠퇴하는 작은 커뮤니티인가요? 책, 웹사이트, 온라인 포럼에서 답을 얻을 수 있나요? 그 포럼에 있는 사람들과 어울리는 게 즐겁나요?

- _간단하게 시작하세요._  
  C++와 Java 같은 프로그래밍 언어는 대규모 팀의 숙련된 프로그래머들이 코드의 실행 효율성을 염두에 두고 전문적인 개발을 위해 설계되었습니다. 결과적으로, 이런 언어들은 이러한 상황에 맞춰 복잡한 부분을 포함하고 있습니다. 하지만, 당신은 프로그래밍을 배우는 것이 주된 관심사입니다. 그런 복잡함은 필요 없습니다. 새로운 초보 프로그래머가 배우고 기억하기 쉽도록 설계된 언어를 선택하세요.

- _재미있게 배우세요._  
  피아노를 배우는 방법을 생각해 보세요. 키를 누르자마자 소리가 들리는 일반적이고 상호작용적인 방식과, 곡 전체를 끝낸 후에 한번에 음을 듣는 "배치(batch)" 모드 중 어떤 것이 더 좋을까요? 분명히, 상호작용적인 모드는 피아노뿐만 아니라 프로그래밍에서도 학습을 더 쉽게 만들어줍니다. 상호작용 모드를 제공하는 언어를 고집하고 그것을 사용하세요.

위 기준을 고려할 때, 제가 추천하는 첫 번째 프로그래밍 언어는 [**Python**](http://python.org/)이나 [**Scheme**](http://www.schemers.org/)입니다. 또 다른 선택은 **JavaScript**인데, 이는 초보자를 위해 완벽하게 설계되었기 때문이 아니라, [Khan Academy의 튜토리얼](https://www.khanacademy.org/computing/cs/programming) 같은 많은 온라인 튜토리얼이 존재하기 때문입니다. 하지만 상황에 따라 다를 수 있으며, 다른 좋은 선택도 있습니다. 만약 나이가 한 자릿수라면 [**Alice**](http://alice.org/), [**Squeak**](http://www.squeak.org/), [**Blockly**](https://blockly-demo.appspot.com/static/apps/index.html) 같은 언어가 더 적합할 수 있습니다(더 나이가 많은 학습자들도 이러한 언어를 즐길 수 있습니다). 가장 중요한 것은 **선택하고 시작하는 것**입니다.

## 부록: 책과 기타 자료

많은 사람들이 어떤 책과 웹 페이지로 학습을 시작해야 하는지 묻습니다. 다시 한 번 강조하지만, **"책만으로는 충분하지 않습니다."** 하지만 다음 자료들을 추천할 수 있습니다:

- **Scheme:**  
  [**《Structure and Interpretation of Computer Programs》** (Abelson & Sussman)](http://www.amazon.com/gp/product/0262011530)는 아마도 컴퓨터 과학에 대한 최고의 입문서일 것입니다. 이 책은 컴퓨터 과학을 이해하는 방법으로 프로그래밍을 가르칩니다. 이 책에 대한 [강의 동영상](http://www.swiss.ai.mit.edu/classes/6.001/abelson-sussman-lectures/)을 온라인에서 볼 수 있으며, [전체 책 내용](http://mitpress.mit.edu/sicp/full-text/book/book.html)도 온라인에서 확인할 수 있습니다. 이 책은 상당히 도전적입니다. 이 책이 너무 어려우면 다른 접근법을 시도해 보세요.

- **Scheme:**  
  [**《How to Design Programs》** (Felleisen 외)](http://www.amazon.com/gp/product/0262062186)는 프로그램을 우아하고 기능적으로 설계하는 방법을 실제로 가르치는 최고의 책 중 하나입니다.

- **Python:**  
  [**《Python Programming: An Intro to CS》** (Zelle)](http://www.amazon.com/gp/product/1887902996)은 Python을 활용한 좋은 입문서입니다.

- **Python:**  
  [**Python.org**](http://python.org/)에서는 여러 온라인 [튜토리얼](http://wiki.python.org/moin/BeginnersGuide)을 제공합니다.

- **Oz:**  
  [**《Concepts, Techniques, and Models of Computer Programming》** (Van Roy & Haridi)](http://www.amazon.com/gp/product/0262220695)은 일부 사람들에게 [SICP](#부록-책과-기타-자료)의 현대판 후속작으로 여겨집니다. 이 책은 프로그래밍의 중요한 아이디어들을 포괄적으로 다루며, [SICP](#부록-책과-기타-자료)보다 읽고 따라가기 쉬운 면이 있습니다. 이 책에서 사용하는 언어 **Oz**는 널리 알려진 언어는 아니지만, 다른 언어를 배우는 기초로 활용됩니다.

## 주석

T. Capey가 아마존의 [**《Complete Problem Solver》**](http://www.amazon.com/exec/obidos/ASIN/0805803092) 페이지에 "Teach Yourself Bengali in 21 Days"와 "Teach Yourself Grammar and Style" 책이 "이 상품을 구매한 고객이 함께 본 상품" 섹션에 포함되어 있다고 알려주셨습니다. 아마도 이 페이지를 방문한 많은 사람들이 이 페이지에서 넘어온 것 같습니다. 히포크라테스(Hippocrates) 관련하여 도움주신 Ross Cohen에게 감사드립니다.
