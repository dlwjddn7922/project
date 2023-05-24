<div align=center>
<img src="https://user-images.githubusercontent.com/79899654/235819020-81b04e26-ff94-406e-b28d-7c73336e0db3.png"></a>

#  YELP 맛집 리뷰
</div>

# YELP 란?

대표적인 지역 기반 소셜네트워크. 여러 도시의 식당, 백화점, 병원 등에 대한 평판을 크라우드 소싱을 이용해 모으는 서비스이다.회원들은 특정 지역의 비즈니스, 서비스, 명소 등에 대한 추천과 리뷰를 공유할 수 있다.

# 문제 정의

배달음식과 맛집탐방이 많아진 요즘 맛집리뷰 사이트와 어플들이 많아지고 있다. 리뷰 평점에 따라 식당에 미치는 영향이 강해지고 있고
평점을 관리하는 매장들이 많아지고있다. 미국기업 YELP를 통해 미국맛집들의 리뷰와 그에따른 기업의 평가를 확인해보겠다.

# YELP의 영향력
옐프의 리뷰에 별점이 하나씩 증가할 때마다 음식점의 매출은 5.4% 증가하는 결과가 나왔다. 
<img src="https://user-images.githubusercontent.com/79899654/235820654-ce90d5fc-46f5-4225-b8c7-442c46fa5fc5.jpg">

출처 : 데일리팝(http://www.dailypop.kr)

# 맛집 리뷰의 영향력

<img src="https://user-images.githubusercontent.com/79899654/235819995-7519ec82-029d-43de-ba73-46417269f175.PNG">
맛집리뷰 이용경험을 조사해본 결과 리뷰서비스의 신뢰도는 62%이상이 매우 신뢰한다고 나타남.

출처 : http://www.hkrecruit.co.kr/news/articleView.html?idxno=23798


- 맛집리뷰가 좋지 않은경우 50%이상이 리뷰가 좋지 않으면 식단에 방문하지 않겠다고 응답함.

출처 : http://www.hkrecruit.co.kr/news/articleView.html?idxno=23798
- 19-49세 성인남여 1,200명 중 86.9%가 ‘소비자 리뷰는 필요하다’고 답했고, 전체 응답자의 78.6%가 제품 구매 시 항상 소비자 리뷰를 확인한다’고 답했습니다.

출처 : https://www.mobiinside.co.kr/2020/01/17/servicereview-review

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
|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|1|	8/11/2016	|"The soft-serve is way too sweet and has a strange Splenda-like aftertaste. The flavors tasted very artificial, and I ended up with a stomach ache when I got home... I really don't recommend this place, your simple Baskin Robbins is much better."|
|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|5|	11/5/2016	|My husband and I stopped here on the way back to Monticello from Westville (Go Sages!). He had a chocolate shake and I had a cookie dough tornado. Both were very tasty and refreshing. What a cute place filled with character. The service was very friendly and efficient. I love small town gems like this!|
|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|5|	8/19/2015	|"Little piece of heaven, the best ice cream shop near Champaign Urbana. Decent prices, superb taste; What else do you need on a hot summer day! This place is cash only, and sometimes you can smell cow dung. Other than that, this place serves far better ice cream than neighboring ice cream parlors (like Jarlings) of Champaign-Urbana."|
|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|2|	7/26/2019|	"Went here for the 1st time tonight. I ordered a turtle tornado. It was excellent. TONS of pecans and lots of flavor. I guess I could be picky and say that it melted incredibly fast. Too bad my wife and son didn't have the same experience. My son ordered a plain chocolate cone. My wife ordered a vanilla cone w/ a chocolate dip. I tasted both, after they said theirs didn't taste very good. I totally agreed. Both were very watery in flavor. My sons had a bit of an icy consistency. Instead of ice cream or custard - they resembled ice milk. Not going back. Jarling's Custard Cup is way, way better."|
|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|4|	3/30/2015	|"Our bike club comes here often year round for evening ice cream cycling excursions from Champaign-Urbana. The staff is always VERY friendly and accommodating. The ice cream is tasty, although I do prefer the fattier taste of custard. All in all, a wonderful place to visit."|
|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|5|	5/18/2018|	Best ice cream in the area! I love their featured flavor of the week! The staff is always very friendly and the service is generally pretty fast!|
|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|5|	5/5/2018|	Delicious ice cream. Best soft serve I've ever had in my entire life. Staff is wonderful and friendly and even though they only have a few flavors it will leave you in a wonderful happy place and life will be good.|
|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|3|	9/4/2014|	"Local Dairy Barn that served your typical traditional American dairy products. The ice cream was itself was so rich that I could taste the milk. If you just simply want an ice cream or something simple, this is definitely a good place to go. But personally I see nothing too special about the place. There's ample amount of parking in their private lot, but expect there to always be full of locals populating the area. When in doubt, just make your own parking spot. I know I did"|
|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|5|	7/22/2016	|The best soft serve hands down...no further explanation needed!! Every flavor...those that are constant or those that change weekly...LOVE. THE. BEST.|
|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|5	|7/6/2016	|Best home made style ice cream. I stop by any time I am near Sidney and make special trips from my home 13 miles away from time to time.|
|https://www.yelp.com/biz/sidney-dairy-barn-sidney	|5|	7/6/2016	|"Definitely have to check out their facebook for the flavor of the week! We were there for coffee flavored and it was delicious. I have to go back to check out the lemon, as I have heard wonderful things about it. Definitely worth the drive if you're looking for something different than custard"|

<img src="https://user-images.githubusercontent.com/79899654/235823416-87e92163-65fb-47e8-8730-343cfa7733a1.PNG"></a>

-리뷰문장이 길다해서 긍정적이고 문장이 짧다고 해서 부정적인 리뷰라고는 말 할 수 없음.

# 긍부정 분석

<img src="https://user-images.githubusercontent.com/79899654/235824184-984f1fbe-3ed4-455b-8239-02aeea32fbb1.PNG"></a>

-평점 4-5점은 긍정 평점1-3점은 부정으로 분류해 분석해봄.

# 평점 데이터

<img src="https://user-images.githubusercontent.com/79899654/235818585-7fc6c992-2f47-442a-b6c2-8929c70b9831.PNG"></a>
 
 -긍정적인 리뷰인  4-5점이 대다수를 차지하고 있음.

# 결론
리뷰의 중요성은 시간이 지날수록 높아지고 있다. 또한 대부분의 고객들은 긍정적인 리뷰를 남기고 있으며, 긍정적인 리뷰가 많은 매장일 수록 기업의 가치와 매출이 높다는걸 확인 할 수 있다.  
