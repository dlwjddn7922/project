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

# 데이터

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
plt.figure(figsize=(12,4))
ax = sns.countplot(business['stars'])
plt.title('Distribution of rating');
