<div align=center>
<img src="https://user-images.githubusercontent.com/79899654/235819020-81b04e26-ff94-406e-b28d-7c73336e0db3.png"></a>

#  YELP 맛집 리뷰
</div>

# YELP 란?

대표적인 지역 기반 소셜네트워크. 여러 도시의 식당, 백화점, 병원 등에 대한 평판을 크라우드 소싱을 이용해 모으는 서비스이다.회원들은 특정 지역의 비즈니스, 서비스, 명소 등에 대한 추천과 리뷰를 공유할 수 있다.

# 문제 정의

배달음식과 맛집탐방이 많아진 요즘 맛집리뷰 사이트와 어플들이 많아지고 있다. 리뷰 평점에 따라 식당에 미치는 영향이 강해지고 있고
평점을 관리하는 매장들이 많아지고있다. 미국기업 YELP를 통해 미국맛집들의 리뷰와 그에따른 기업의 평가를 확인해보겠다.

# 맛집 리뷰의 영향력

- 맛집리뷰 이용경험을 조사해본 결과 리뷰서비스의 신뢰도는 62%이상이 매우 신뢰한다고 나타났다.
 <img scr="https://user-images.githubusercontent.com/79899654/235819995-7519ec82-029d-43de-ba73-46417269f175.PNG"></a>
- 맛집리뷰가 좋지 않은경우 50%이상이 리뷰가 좋지 않으면 식단에 방문하지 않겠다고 응답했다.
- 리뷰평점이 높을수록 기업의 가치도 높다고 예측할 수 있다는 결과가 나왔다.
 <출처:http://www.hkrecruit.co.kr/news/articleView.html?idxno=23798>
- 19-49세 성인남여 1,200명 중 86.9%가 ‘소비자 리뷰는 필요하다’고 답했고, 전체 응답자의 78.6%가 제품 구매 시 항상 소비자 리뷰를 확인한다’고 답했습니다.
 <출처:https://www.mobiinside.co.kr/2020/01/17/servicereview-review>

# 데이터 소개

- kaggle 사이트에서 business review 데이터에서 미국기업 yelp를 사용한 데이터를 사용하였다. (https://www.kaggle.com/code/sudhirnl7/basic-exploration-of-business-review-at-yelp-com#Review)
- kaggle 사이트에서 Yelp Restaurant Reviews 데이터를 사용하였다 (https://www.kaggle.com/datasets/farukalam/yelp-restaurant-reviews)

# 데이터

<img src="https://www.kaggleusercontent.com/kf/2594553/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..gp4FvRrugxdz-OahmDcbgA.WxX51E0OnVK7udFMbQNDKnaPMWtok5_YREg_MJ6koxjf1YMXBwuflT0CxHka7pPgUlrDBpuaCRPlqckmkX33gpEAHGLbntBxztyRc7Da94azy4RAt-lXZrHeuYxNq5ejRvBruBbvvagL7VjBxQgCmZnQFWx1NyyF49VIHV14YI7s0YanYvsnIkRdiLSzM3GZI42AgBHyvgWt562TXb7l478rCMg-CeVC9oMDf2gj3rY1OGX3s6R1um4tFAFnKHVQ4cDx74UBtkziumKDBWa9ax49uARWez0a-eXjyNtPf18HRK25weonO-cO5Z6RbNt3tTryCG10YaQtgzN3OtD5uQdr3fFpVotQB7qmUjU3wl9CdaWVhIgcEi45HI2quXeWUMtaauwpilX0Z3Dr2mPUV2fyKZpbdHxOOM2rhSPkQGqSd9zA8QmVOpO4jXiFGJhu23po3LakBfCMdTQFyr66eTIjtjW0u_d0hkfpcRR5sFts4d2ibOa3BUZGidw-RKPbx8EgP-EIJIQkL3WU8uvlMI5qEfkBX9GYrMguCbjFlZv9lwJDYZovW9pPPr4U1_x47Lu_U86uoYRpoAuT2zPnmsIezSyBMFBvaJSOWeqE0UP5SCGzHzCNi-LZVG8RDEiJjVhs3q-0CJLgurQwsGFvDVxLzgMBKI52A9CrTxYT0WhsTaNwjFVom-s_ppDBFdXabdilQiZZlfSJ7hf5Wis2NQ.0rnRMB18uhU2QbsHQhlY8g/__results___files/__results___9_0.png"></a>
- 대부분의 유저들은 평점을 4점이상을 주고있다.

<img src="https://www.kaggleusercontent.com/kf/2594553/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..gp4FvRrugxdz-OahmDcbgA.WxX51E0OnVK7udFMbQNDKnaPMWtok5_YREg_MJ6koxjf1YMXBwuflT0CxHka7pPgUlrDBpuaCRPlqckmkX33gpEAHGLbntBxztyRc7Da94azy4RAt-lXZrHeuYxNq5ejRvBruBbvvagL7VjBxQgCmZnQFWx1NyyF49VIHV14YI7s0YanYvsnIkRdiLSzM3GZI42AgBHyvgWt562TXb7l478rCMg-CeVC9oMDf2gj3rY1OGX3s6R1um4tFAFnKHVQ4cDx74UBtkziumKDBWa9ax49uARWez0a-eXjyNtPf18HRK25weonO-cO5Z6RbNt3tTryCG10YaQtgzN3OtD5uQdr3fFpVotQB7qmUjU3wl9CdaWVhIgcEi45HI2quXeWUMtaauwpilX0Z3Dr2mPUV2fyKZpbdHxOOM2rhSPkQGqSd9zA8QmVOpO4jXiFGJhu23po3LakBfCMdTQFyr66eTIjtjW0u_d0hkfpcRR5sFts4d2ibOa3BUZGidw-RKPbx8EgP-EIJIQkL3WU8uvlMI5qEfkBX9GYrMguCbjFlZv9lwJDYZovW9pPPr4U1_x47Lu_U86uoYRpoAuT2zPnmsIezSyBMFBvaJSOWeqE0UP5SCGzHzCNi-LZVG8RDEiJjVhs3q-0CJLgurQwsGFvDVxLzgMBKI52A9CrTxYT0WhsTaNwjFVom-s_ppDBFdXabdilQiZZlfSJ7hf5Wis2NQ.0rnRMB18uhU2QbsHQhlY8g/__results___files/__results___11_1.png"></a>
- 우리가 흔히 아는 기업일 수록 평가가 많다는걸 알 수 있다.

<img src="https://www.kaggleusercontent.com/kf/2594553/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..gp4FvRrugxdz-OahmDcbgA.WxX51E0OnVK7udFMbQNDKnaPMWtok5_YREg_MJ6koxjf1YMXBwuflT0CxHka7pPgUlrDBpuaCRPlqckmkX33gpEAHGLbntBxztyRc7Da94azy4RAt-lXZrHeuYxNq5ejRvBruBbvvagL7VjBxQgCmZnQFWx1NyyF49VIHV14YI7s0YanYvsnIkRdiLSzM3GZI42AgBHyvgWt562TXb7l478rCMg-CeVC9oMDf2gj3rY1OGX3s6R1um4tFAFnKHVQ4cDx74UBtkziumKDBWa9ax49uARWez0a-eXjyNtPf18HRK25weonO-cO5Z6RbNt3tTryCG10YaQtgzN3OtD5uQdr3fFpVotQB7qmUjU3wl9CdaWVhIgcEi45HI2quXeWUMtaauwpilX0Z3Dr2mPUV2fyKZpbdHxOOM2rhSPkQGqSd9zA8QmVOpO4jXiFGJhu23po3LakBfCMdTQFyr66eTIjtjW0u_d0hkfpcRR5sFts4d2ibOa3BUZGidw-RKPbx8EgP-EIJIQkL3WU8uvlMI5qEfkBX9GYrMguCbjFlZv9lwJDYZovW9pPPr4U1_x47Lu_U86uoYRpoAuT2zPnmsIezSyBMFBvaJSOWeqE0UP5SCGzHzCNi-LZVG8RDEiJjVhs3q-0CJLgurQwsGFvDVxLzgMBKI52A9CrTxYT0WhsTaNwjFVom-s_ppDBFdXabdilQiZZlfSJ7hf5Wis2NQ.0rnRMB18uhU2QbsHQhlY8g/__results___files/__results___53_1.png"></a>
- 시간이 지날수록 리뷰를 작성하는 사람이 많아지고 리뷰의 중요성이 높아지고있다.

# 리뷰 데이터

|Yelp URL|Rating|Date|Review text|
|---|---|---|---|
|레스토랑 주소URL|평점|날짜|리뷰 글|

<img src="https://user-images.githubusercontent.com/79899654/235818583-6205bca6-7e54-4ce7-9463-6a519acc1168.PNG"></a>

# 평점 데이터

<img src="https://user-images.githubusercontent.com/79899654/235818585-7fc6c992-2f47-442a-b6c2-8929c70b9831.PNG"></a>
 
 -평점 5점이 50%이상이걸 알 수 있다.

# 결론
리뷰의 중요성은 시간이 지날수록 높아지고 있고, 리뷰가 좋은 기업일 수록 가치가 높은 기업으로 나타났다.
