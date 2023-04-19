<div align=center>
<img src="http://file3.instiz.net/data/file3/2018/02/04/d/c/5/dc516762058e13cf88cc753ccbd2b140.jpg"></a>

# 맛집 리뷰
</div>


# 문제 정의

배달음식과 맛집탐방이 많아진 요즘 맛집리뷰 사이트와 어플들이 많아지고 있다. 리뷰 평점에 따라 식당에 미치는 영향이 강해지고 있고
평점을 관리하는 매장들이 많아지고있다. 미국기업 yelp를 통해 미국맛집들의 리뷰와 그에따른 기업의 평가를 확인해보겠다.



# 맛집 리뷰의 영향력

- 맛집리뷰 이용경험을 조사해본 결과 리뷰서비스의 신뢰도는 62%이상이 매우 신뢰한다고 나타났다
- 맛집리뷰가 좋지 않은경우 50%이상이 리뷰가 좋지 않으면 식단에 방문하지 않겠다고 응답했다.
- 리뷰평점이 높을수록 기업의 가치도 높다고 예측할 수 있다는 결과가 나왔다.

# 데이터 소개

- kaggle 사이트에서 business review 데이터에서 미국기업 yelp를 사용한 데이터를 사용하였다. (https://www.kaggle.com/code/sudhirnl7/basic-exploration-of-business-review-at-yelp-com#Review)
- kaggle 사이트에서 Restaurant Customer Reviews 데이터를 사용하였다 (https://www.kaggle.com/datasets/vigneshwarsofficial/reviews)

# 데이터

<img src="https://www.kaggleusercontent.com/kf/2594553/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..gp4FvRrugxdz-OahmDcbgA.WxX51E0OnVK7udFMbQNDKnaPMWtok5_YREg_MJ6koxjf1YMXBwuflT0CxHka7pPgUlrDBpuaCRPlqckmkX33gpEAHGLbntBxztyRc7Da94azy4RAt-lXZrHeuYxNq5ejRvBruBbvvagL7VjBxQgCmZnQFWx1NyyF49VIHV14YI7s0YanYvsnIkRdiLSzM3GZI42AgBHyvgWt562TXb7l478rCMg-CeVC9oMDf2gj3rY1OGX3s6R1um4tFAFnKHVQ4cDx74UBtkziumKDBWa9ax49uARWez0a-eXjyNtPf18HRK25weonO-cO5Z6RbNt3tTryCG10YaQtgzN3OtD5uQdr3fFpVotQB7qmUjU3wl9CdaWVhIgcEi45HI2quXeWUMtaauwpilX0Z3Dr2mPUV2fyKZpbdHxOOM2rhSPkQGqSd9zA8QmVOpO4jXiFGJhu23po3LakBfCMdTQFyr66eTIjtjW0u_d0hkfpcRR5sFts4d2ibOa3BUZGidw-RKPbx8EgP-EIJIQkL3WU8uvlMI5qEfkBX9GYrMguCbjFlZv9lwJDYZovW9pPPr4U1_x47Lu_U86uoYRpoAuT2zPnmsIezSyBMFBvaJSOWeqE0UP5SCGzHzCNi-LZVG8RDEiJjVhs3q-0CJLgurQwsGFvDVxLzgMBKI52A9CrTxYT0WhsTaNwjFVom-s_ppDBFdXabdilQiZZlfSJ7hf5Wis2NQ.0rnRMB18uhU2QbsHQhlY8g/__results___files/__results___9_0.png"></a>
- 대부분의 유저들은 평점을 4점이상을 주고있다.

<img src="https://www.kaggleusercontent.com/kf/2594553/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..gp4FvRrugxdz-OahmDcbgA.WxX51E0OnVK7udFMbQNDKnaPMWtok5_YREg_MJ6koxjf1YMXBwuflT0CxHka7pPgUlrDBpuaCRPlqckmkX33gpEAHGLbntBxztyRc7Da94azy4RAt-lXZrHeuYxNq5ejRvBruBbvvagL7VjBxQgCmZnQFWx1NyyF49VIHV14YI7s0YanYvsnIkRdiLSzM3GZI42AgBHyvgWt562TXb7l478rCMg-CeVC9oMDf2gj3rY1OGX3s6R1um4tFAFnKHVQ4cDx74UBtkziumKDBWa9ax49uARWez0a-eXjyNtPf18HRK25weonO-cO5Z6RbNt3tTryCG10YaQtgzN3OtD5uQdr3fFpVotQB7qmUjU3wl9CdaWVhIgcEi45HI2quXeWUMtaauwpilX0Z3Dr2mPUV2fyKZpbdHxOOM2rhSPkQGqSd9zA8QmVOpO4jXiFGJhu23po3LakBfCMdTQFyr66eTIjtjW0u_d0hkfpcRR5sFts4d2ibOa3BUZGidw-RKPbx8EgP-EIJIQkL3WU8uvlMI5qEfkBX9GYrMguCbjFlZv9lwJDYZovW9pPPr4U1_x47Lu_U86uoYRpoAuT2zPnmsIezSyBMFBvaJSOWeqE0UP5SCGzHzCNi-LZVG8RDEiJjVhs3q-0CJLgurQwsGFvDVxLzgMBKI52A9CrTxYT0WhsTaNwjFVom-s_ppDBFdXabdilQiZZlfSJ7hf5Wis2NQ.0rnRMB18uhU2QbsHQhlY8g/__results___files/__results___11_1.png"></a>
- 우리가 흔히 아는 기업일 수록 평가가 많다는걸 알 수 있다.

<img src="https://www.kaggleusercontent.com/kf/2594553/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..gp4FvRrugxdz-OahmDcbgA.WxX51E0OnVK7udFMbQNDKnaPMWtok5_YREg_MJ6koxjf1YMXBwuflT0CxHka7pPgUlrDBpuaCRPlqckmkX33gpEAHGLbntBxztyRc7Da94azy4RAt-lXZrHeuYxNq5ejRvBruBbvvagL7VjBxQgCmZnQFWx1NyyF49VIHV14YI7s0YanYvsnIkRdiLSzM3GZI42AgBHyvgWt562TXb7l478rCMg-CeVC9oMDf2gj3rY1OGX3s6R1um4tFAFnKHVQ4cDx74UBtkziumKDBWa9ax49uARWez0a-eXjyNtPf18HRK25weonO-cO5Z6RbNt3tTryCG10YaQtgzN3OtD5uQdr3fFpVotQB7qmUjU3wl9CdaWVhIgcEi45HI2quXeWUMtaauwpilX0Z3Dr2mPUV2fyKZpbdHxOOM2rhSPkQGqSd9zA8QmVOpO4jXiFGJhu23po3LakBfCMdTQFyr66eTIjtjW0u_d0hkfpcRR5sFts4d2ibOa3BUZGidw-RKPbx8EgP-EIJIQkL3WU8uvlMI5qEfkBX9GYrMguCbjFlZv9lwJDYZovW9pPPr4U1_x47Lu_U86uoYRpoAuT2zPnmsIezSyBMFBvaJSOWeqE0UP5SCGzHzCNi-LZVG8RDEiJjVhs3q-0CJLgurQwsGFvDVxLzgMBKI52A9CrTxYT0WhsTaNwjFVom-s_ppDBFdXabdilQiZZlfSJ7hf5Wis2NQ.0rnRMB18uhU2QbsHQhlY8g/__results___files/__results___53_1.png"></a>
- 시간이 지날수록 리뷰를 작성하는 사람이 많아지고 리뷰의 중요성이 높아지고있다.

# 리뷰 데이터

|-|review_ID|user_id	|business_id|stars|date|text|useful|
|-|--------|--------|--------|------|------|----|-----------|
|0|	vkVSCC7xljjrAI4UGfnKEQ|bv2nCi5Qv5vroFiqKGopiw|AEx2SYEUJmTxVVB18LlCwA|5|2016-05-28|Super simple place but amazing nonetheless. It...|0|
|1|n6QzIUObkYshz4dz2QRJTw|bv2nCi5Qv5vroFiqKGopiw|VR6GpWIda3SfvPC-lg9H3w|5|2016-05-28|Small unassuming place that changes their menu...|0|
|2|MV3CcKScW05u5LVfF6ok0g	|bv2nCi5Qv5vroFiqKGopiw|CKC0-MOWMqoeWf6s-szl8g|5|2016-05-28|Lester's is located in a beautiful neighborhoo...|0|
|3|IXvOzsEMYtiJI0CARmj77Q|bv2nCi5Qv5vroFiqKGopiw|ACFtxLv8pGrrxMm6EgjreA|4|2016-05-28|Love coming here. Yes the place always needs t...|0|
|4|L_9BTb55X0GDtThi6GlZ6w|bv2nCi5Qv5vroFiqKGopiw|s2I_Ni76bjJNK9yG60iD-Q|4|2016-05-28|Had their chocolate almond croissant and it wa...|0|

(review.xlxs)
# 결론
리뷰의 중요성은 시간이 지날수록 높아지고 있고, 리뷰가 좋은 기업일 수록 가치가 높은 기업으로 나타났다.
