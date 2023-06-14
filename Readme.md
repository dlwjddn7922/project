<div align=center>
<img src="https://user-images.githubusercontent.com/79899654/235819020-81b04e26-ff94-406e-b28d-7c73336e0db3.png"></a>

#  YELP 맛집 리뷰
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

# 개발 환경
<img src="https://github.com/dlwjddn7922/project/assets/79899654/a64eecae-3caa-4f66-ae2b-e802c83dd416">

# 데이터 소개

- kaggle 사이트에서 business review 데이터에서 미국기업 yelp를 사용한 데이터를 사용하였다. (https://www.kaggle.com/code/sudhirnl7/basic-exploration-of-business-review-at-yelp-com#Review)
- kaggle 사이트에서 Yelp Restaurant Reviews 데이터를 사용하였다 (https://www.kaggle.com/datasets/farukalam/yelp-restaurant-reviews)

# 데이터
<img src="https://www.kaggleusercontent.com/kf/2594553/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..gp4FvRrugxdz-OahmDcbgA.WxX51E0OnVK7udFMbQNDKnaPMWtok5_YREg_MJ6koxjf1YMXBwuflT0CxHka7pPgUlrDBpuaCRPlqckmkX33gpEAHGLbntBxztyRc7Da94azy4RAt-lXZrHeuYxNq5ejRvBruBbvvagL7VjBxQgCmZnQFWx1NyyF49VIHV14YI7s0YanYvsnIkRdiLSzM3GZI42AgBHyvgWt562TXb7l478rCMg-CeVC9oMDf2gj3rY1OGX3s6R1um4tFAFnKHVQ4cDx74UBtkziumKDBWa9ax49uARWez0a-eXjyNtPf18HRK25weonO-cO5Z6RbNt3tTryCG10YaQtgzN3OtD5uQdr3fFpVotQB7qmUjU3wl9CdaWVhIgcEi45HI2quXeWUMtaauwpilX0Z3Dr2mPUV2fyKZpbdHxOOM2rhSPkQGqSd9zA8QmVOpO4jXiFGJhu23po3LakBfCMdTQFyr66eTIjtjW0u_d0hkfpcRR5sFts4d2ibOa3BUZGidw-RKPbx8EgP-EIJIQkL3WU8uvlMI5qEfkBX9GYrMguCbjFlZv9lwJDYZovW9pPPr4U1_x47Lu_U86uoYRpoAuT2zPnmsIezSyBMFBvaJSOWeqE0UP5SCGzHzCNi-LZVG8RDEiJjVhs3q-0CJLgurQwsGFvDVxLzgMBKI52A9CrTxYT0WhsTaNwjFVom-s_ppDBFdXabdilQiZZlfSJ7hf5Wis2NQ.0rnRMB18uhU2QbsHQhlY8g/__results___files/__results___11_1.png"></a>
- 우리가 흔히 아는 기업일 수록 평가가 많다는걸 알 수 있다.

<img src="https://www.kaggleusercontent.com/kf/2594553/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..gp4FvRrugxdz-OahmDcbgA.WxX51E0OnVK7udFMbQNDKnaPMWtok5_YREg_MJ6koxjf1YMXBwuflT0CxHka7pPgUlrDBpuaCRPlqckmkX33gpEAHGLbntBxztyRc7Da94azy4RAt-lXZrHeuYxNq5ejRvBruBbvvagL7VjBxQgCmZnQFWx1NyyF49VIHV14YI7s0YanYvsnIkRdiLSzM3GZI42AgBHyvgWt562TXb7l478rCMg-CeVC9oMDf2gj3rY1OGX3s6R1um4tFAFnKHVQ4cDx74UBtkziumKDBWa9ax49uARWez0a-eXjyNtPf18HRK25weonO-cO5Z6RbNt3tTryCG10YaQtgzN3OtD5uQdr3fFpVotQB7qmUjU3wl9CdaWVhIgcEi45HI2quXeWUMtaauwpilX0Z3Dr2mPUV2fyKZpbdHxOOM2rhSPkQGqSd9zA8QmVOpO4jXiFGJhu23po3LakBfCMdTQFyr66eTIjtjW0u_d0hkfpcRR5sFts4d2ibOa3BUZGidw-RKPbx8EgP-EIJIQkL3WU8uvlMI5qEfkBX9GYrMguCbjFlZv9lwJDYZovW9pPPr4U1_x47Lu_U86uoYRpoAuT2zPnmsIezSyBMFBvaJSOWeqE0UP5SCGzHzCNi-LZVG8RDEiJjVhs3q-0CJLgurQwsGFvDVxLzgMBKI52A9CrTxYT0WhsTaNwjFVom-s_ppDBFdXabdilQiZZlfSJ7hf5Wis2NQ.0rnRMB18uhU2QbsHQhlY8g/__results___files/__results___53_1.png"></a>
- 시간이 지날수록 리뷰를 작성하는 사람이 많아지고 리뷰의 중요성이 높아지고있다.

# 리뷰 데이터

|Yelp URL|Rating|Date|Review text|
|---|---|---|---|
|레스토랑 주소URL|평점|날짜|리뷰 글|

|Yelp URL|Rating|Date|Review text|
|---|---|---|---|
|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|5	|1/22/2022	All I |can say is they have very good ice cream I would for sure recommend their cookies and creme ice cream it is very good|
|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|4|	6/26/2022|	Nice little local place for ice cream.My favorite is their pumpkin shake ( Fall season special).( My Sweetness tolerance is low) Their LARGE SIZE ice cream usually seems too sweet after having ice cream for a while. But love their pina colada. So refreshing. Their Banana Split is good too.|
|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|5|	8/7/2021	|A delicious treat on a hot day! Staff was very friendly and helpful-- gave us a sample and let us order a little earlier than open.|
|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|4|	7/28/2016|	"This was great service and a fun crew! I got the banana cream pie with chocolate ice cream. I loved the flavor of this. It had freshly cut bananas, graham crackers and chocolate ice cream. YUM!! The only thing that I noticed is that it melted pretty fast and it's a bit icy. I like creamier ice cream (so it had a bit more overrun that I prefer), but overall, was delicious!"|
|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|5|	6/23/2015|	"This is one of my favorite places to get ice cream in the CU area. It's a bit of drive, but it is worth it. It's about 10 minutes from the far side of Urbana. Getting there is really easy. The atmosphere of the Dairy Barn is very kid friendly. There are many tables set up so that you can sit and enjoy the ice cream. When my friends and I went, the line was about a 20 minute wait, but it didn't seem like any time at all. An older gentlemen, I presume the manager or owner, was giving out samples to the entire line. You could tell that he took pride in the product he made and was excited to share it with everyone. The special that night was cappuccino ice cream. I added in cookie dough to make a ""tornado"" which is a blizzard like ice cream treat. It was so quite refreshing and was a nice treat on a humid night. The Dairy barn is a must go!"|
|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|5|	5/1/2019	|"I've been coming to this ice cream stand since I was a little girl back in the 1970's. (Yes, it's been here for that long! Just not under the same ownership.) But not much has changed in those years in regards to their basic ice cream. It is a great family place! They are always accommodating when we want to tweak the menu item a bit :-) I love the rotating, special flavor of the week! Keep an eye on the Facebook page for that. It's always a joy to see the near constant long line. Shows how successful a small town business can be. If you are truly passionate about supporting small business, stay away from those franchises that make their ice cream at some corporate factory and come get some made fresh soft serve from your truly local business!!"|
# 평점 데이터

<img src="https://user-images.githubusercontent.com/79899654/235818585-7fc6c992-2f47-442a-b6c2-8929c70b9831.PNG"></a>
 
 -긍정적인 리뷰인  4-5점이 대다수를 차지하고 있음.

<img src="https://user-images.githubusercontent.com/79899654/235823416-87e92163-65fb-47e8-8730-343cfa7733a1.PNG"></a>

-리뷰문장이 길다해서 긍정적이고 문장이 짧다고 해서 부정적인 리뷰라고는 말 할 수 없음.

# 긍부정 분석

<img src="https://user-images.githubusercontent.com/79899654/235824184-984f1fbe-3ed4-455b-8239-02aeea32fbb1.PNG"></a>

-평점 4-5점은 긍정 평점1-3점은 부정으로 분류해 분석해봄.

 <img src="https://github.com/dlwjddn7922/project/assets/79899654/8a00ad79-ac33-4f54-8083-cdea8127f61f"></a>
 
-평점 4-5점은 긍정 1-3점은 부정으로 분류하여 파이차트로 나타냄



# 결론
리뷰의 중요성은 시간이 지날수록 높아지고 있다. 또한 대부분의 고객들은 긍정적인 리뷰를 남기고 있으며, 긍정적인 리뷰가 많은 매장일 수록 기업의 가치와 매출이 높다는걸 확인 할 수 있다.</br>

