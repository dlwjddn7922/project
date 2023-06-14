<div align=center>
<img src="https://user-images.githubusercontent.com/79899654/235819020-81b04e26-ff94-406e-b28d-7c73336e0db3.png"></a>

#  YELP 맛집 리뷰
<img src="https://img.shields.io/badge/tensorflow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white"/>
<img src="https://img.shields.io/badge/matplotlib-3776AB?style=flat-square&logo=matplotlib&logoColor=white"/>
<img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white"/>
<img src="https://img.shields.io/badge/numpy-013243?style=flat-square&logo=numpy&logoColor=white"/>
<img src="https://img.shields.io/badge/torch-EE4C2C?style=flat-square&logo=torch&logoColor=white"/>
<img src="https://img.shields.io/badge/transformers-409FFF?style=flat-square&logo=transformers&logoColor=white"/>
<img src="https://img.shields.io/badge/scikit-learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white"/>
</div>

# YELP 란?

대표적인 지역 기반 소셜네트워크. 여러 도시의 식당, 백화점, 병원 등에 대한 평판을 크라우드 소싱을 이용해 모으는 서비스이다.회원들은 특정 지역의 비즈니스, 서비스, 명소 등에 대한 추천과 리뷰를 공유할 수 있다.</br>
옐프는 2004년 미국에서 출시한 미국 최대 ‘지역 리뷰’ 사이트로 미국뿐만 아니라 전 세계 32개국에서 서비스를 하고 있는 중이다. 2016년 말 기준으로 월 액티브 유저 수는 1억 3500만 명에 달하고 있으며 10년간 쌓인 누적 데이터 수는 1억 2000만 건에 달한다. 이중 쇼핑과 식당이 40%를 차지하고 있어 미국인들 사이에서는 ‘맛집 찾기는 역시 YELP’로 통한다.

출처 : 데일리팝(http://www.dailypop.kr/news/articleView.html?idxno=37410)

# YELP의 영향력

YELP는 온라인 플랫폼을 구축해 소비자와 로컬 매장의 사업자를 연결하고 있는 옐프는 구축된 플랫폼을 활용해 사용자에게 필요한 데이터를 제공하고, 사업자에게는 고객 유지와 매상 증가를 도와주고 있다.</br>
7년간의 통계자료를 분석한 결과 YELP의 리뷰에 별점이 하나씩 증가할 때마다 음식점의 매출이 5.4% 증가하는 결과가 나왔다고 할 정도로 영향력이 커졌습니다.
지난해 말 기준 YELP의 누적 리뷰 수는 2억2400만개입니다.</br></br>

YELP 외에도 많은 리뷰사이트가  존재하는데 리뷰 사이트 이용자들의 이용경험을 조사해본 결과 리뷰서비스의 신뢰도는 62%이상이 매우 신뢰한다고 나타났고,
리뷰가 좋지 않은 경우 50%이상이 식당에 방문하지 않겠다고 응답했다.

<img src="https://user-images.githubusercontent.com/79899654/235819995-7519ec82-029d-43de-ba73-46417269f175.PNG">

출처 : 데일리팝(http://www.dailypop.kr/news/articleView.html?idxno=37410)</br>
출처 : http://www.hkrecruit.co.kr/news/articleView.html?idxno=23798


# 문제 정의

배달음식과 맛집탐방이 많아진 요즘 맛집리뷰 사이트와 어플들이 많아지고 있다. 리뷰 평점에 따라 식당에 미치는 영향이 강해지고 있고
평점을 관리하는 매장들이 많아지고있다. 미국기업 YELP를 통해 미국맛집들의 리뷰와 그에따른 기업의 평가를 확인하고, Keggle에서 제공하는 YELP APP 리뷰 데이터를 바탕으로
리뷰의 긍정 또는 부정을 예측하는 인공지는 모델을 개발 하고자 한다.

# 데이터 소개

- kaggle 사이트에서 business review 데이터에서 미국기업 yelp를 사용한 데이터를 사용하였다. (https://www.kaggle.com/code/sudhirnl7/basic-exploration-of-business-review-at-yelp-com#Review)
- kaggle 사이트에서 Yelp Restaurant Reviews 데이터를 사용하였다 (https://www.kaggle.com/datasets/farukalam/yelp-restaurant-reviews)

# 리뷰 데이터

|Yelp URL|Rating|Date|Review text|
|---|---|---|---|
|레스토랑 주소URL|평점|날짜|리뷰 글|

|Index|Yelp URL|Rating|Date|Review text|
|---|---|---|---|---|
|1|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|5	|1/22/2022	All I |can say is they have very good ice cream I would for sure recommend their cookies and creme ice cream it is very good|
|2|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|4|	6/26/2022|	Nice little local place for ice cream.My favorite is their pumpkin shake ( Fall season special).( My Sweetness tolerance is low) Their LARGE SIZE ice cream usually seems too sweet after having ice cream for a while. But love their pina colada. So refreshing. Their Banana Split is good too.|
|3|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|5|	8/7/2021	|A delicious treat on a hot day! Staff was very friendly and helpful-- gave us a sample and let us order a little earlier than open.|
|4|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|4|	7/28/2016|	"This was great service and a fun crew! I got the banana cream pie with chocolate ice cream. I loved the flavor of this. It had freshly cut bananas, graham crackers and chocolate ice cream. YUM!! The only thing that I noticed is that it melted pretty fast and it's a bit icy. I like creamier ice cream (so it had a bit more overrun that I prefer), but overall, was delicious!"|
|... | ... | ... | ... |... |
|19893|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|3	|1/22/2022	All I |Delicious. We got a breakfast sandwich here and it was very good. Also I got some sort of lemon tart dessert that was also delicious.|
|19894|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|4|	9/3/2019|	Great gelato and great milkshakes. Stopped here after Din Tai Fung closed so some dessert and it was the real deal. I ordered the Oreo milkshake but everyone I was with had the gelato and loved it.|
|19895|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|5|	8/7/2021	|"Its hard not to order everything when I come here because its so good. You can also order on Instacart for delivery. They always get my order correct which I appreciate"|


- 전체데이터는 19895개이고, 긍정(4-5점)은 15330개, 부정(1-2점)은 2497, 중립을 의미하는 3점은 2069개이다.


# 리뷰데이터 가공

|Index|Review text|Rating|
|---|---|---|
|1|can say is they have very good ice cream I would for sure recommend their cookies and creme ice cream it is very good|5|
|2|A delicious treat on a hot day! Staff was very friendly and helpful-- gave us a sample and let us order a little earlier than open.|5|
|3|Nice little local place for ice cream.My favorite is their pumpkin shake ( Fall season special).( My Sweetness tolerance is low) Their LARGE SIZE ice cream usually seems too sweet after having ice cream for a while. But love their pina colada. So refreshing. Their Banana Split is good too.|4|
|4| "This is one of my favorite places to get ice cream in the CU area. It's a bit of drive, but it is worth it. It's about 10 minutes from the far side of Urbana. Getting there is really easy. The atmosphere of the Dairy Barn is very kid friendly. There are many tables set up so that you can sit and enjoy the ice cream. When my friends and I went, the line was about a 20 minute wait, but it didn't seem like any time at all. An older gentlemen, I presume the manager or owner, was giving out samples to the entire line. You could tell that he took pride in the product he made and was excited to share it with everyone. The special that night was cappuccino ice cream. I added in cookie dough to make a ""tornado"" which is a blizzard like ice cream treat. It was so quite refreshing and was a nice treat on a humid night. The Dairy barn is a must go!"|5|
|... | ... | ... |
|17826|I love this shop! I started buying pints from here last year prior to the scoop shop opening and I have never had a flavor I didn't love. I stopped by the shop today and the women working.|4|
|17827|	Easily my favorite ice cream in Madison. I had enjoyed a mini waffle cone of the "They See Me Rollin'" flavor and it was too good! We also tried the orange pistachio chip (okay) and the "it's brownies b*tch" (really good). Definitely coming back for more.|4|
|17828|We've been buying ice cream from Ice Cream Social (Katrina) for the last several months, and it's *easily the best ice cream in Madison.|5|

 -중립 데이터인 3점을 제거하여 17828개의 데이터만 남겼다.
 
 # 긍부정 분석
 
<img src="https://github.com/dlwjddn7922/project/assets/79899654/b2ab58e6-5703-4685-82fc-005aecc4893b">

-긍부정 데이터 2000건만 추출하여 돌려본 결과 0.06 loss와 0.95 Accuracy가 나왔다.

<img src="https://github.com/dlwjddn7922/project/assets/79899654/13e1fb28-bf90-4c25-9f09-9dd92b881a19">

- 이와같이 loss가 계속 떨어지는걸 볼 수 있다.

<img src="https://github.com/dlwjddn7922/project/assets/79899654/cc476ee1-317e-4528-a038-e082aad3e930">

- Accuracy는 시간이 지날수록 증가하는 걸 볼 수 있다.

<img src="https://github.com/dlwjddn7922/project/assets/79899654/95b61880-de58-4a50-a2c2-73db636a8283">

-전체 데이터인 17828개를 넣어서 돌려본 결과 2000개 보단 낮은 0.86 Accuracy가 나왔다.
 
# 결론
대부분의 고객들은 긍정적인 리뷰를 남기고 있으며, 리뷰의 길이와는 관계없이 평점이 매겨지고있고 매장들이 리뷰의 영향을 많이 받는걸 알 수 있었다. 다음에 분석을 한다면 다른 주제로 더 많은 데이터와 다양한 관점으로 긍부정을 분석해 보고 싶다.</br>

