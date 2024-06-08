# 시간표 도와줄게유 서비스 소개

모든 연세인이 지금까지 수강신청을 하면서, 에브리타임과 연세포털을 계속 번갈아가면서 쓰는 것이 참 불편하다고 느낄 것입니다. 

에브리타임으로 과목 찾고 -> 포털에서 마일리지 확인하고 -> 에브리타임 시간표에 넣고 -> 과목 찾고 -> 마일리지 확인하고 -> 한 번씩은 마일리지가 초과되어 다시 다른 과목 찾고.. 

정말 번거로운 일이 아닐 수 없습니다. 여러분도 공감되시죠?

그래서 저는 이 불편한 과정들을 "정말 빠르고 편리하게 한 페이지 내에서 해결"할 수 있는 유일무이한 서비스, '시간표 도와줄게유'를 기획하게 되었습니다.

이 서비스는 먼저 연세포털에서 '수강 편람' 및 각각의 과목들에 대한 3~4개년 '마일리지'를 받아 오고, 에브리타임에서는 '강의평 (별점)'과 '학점을 잘 주시는 정도, 과제량, 조별 활동 빈도 수'를 받아와 Database에 저장합니다. 

이후 과목을 시간표에 넣을 때 마우스 커서를 과목 위에 올리기만 하면 Database에 저장된 정보를 토대로 수강을 위해 넣어야 하는 평균 마일리지, 별점 및 사용자가 선택한 기준에 따라 헬강인지 꿀강인지를 알 수 있도록 팝업이 뜨게 제작할 계획입니다. 이러면 사용자는 시간표를 짜느라 에브리타임과 연세포털을 넘나들지 않아도 되고, 과목을 선택하고 지우는 과정에서 마일리지 때문에 스트레스를 받을 일도 없습니다. 이것만으로도 사용자는 엄청난 편리함을 느끼게 될 것입니다.

이에 더해, 시간표 짜기 기능에 엄청나게 편리한 기능인 공강 만들기를 추가했습니다. 필수적으로 들어야 하는 전공 과목을 넣고 나면, 사용자가 설정한 공강 요일을 토대로 다른 요일의 과목들만 추천하게 됩니다. 이는 모두에게, 특히 통학 시간이 긴 학우들에게 메리트가 있을 것입니다.

마지막으로 수강편람에는 모든 과목들이 들어있기 때문에 에브리타임에는 없는 '대학원생을 위한 시간표 서비스'까지도 구현할 수 있는 만큼, 이 서비스는 엄청난 확장성을 가지고 있습니다. 하지만 아직은 사용자의 피드백에 따라 확장 방향성을 고려하고 있는, 그런 잠재력 있는 서비스라고 할 수 있습니다. 감사합니다.
<p align="center">
<img width="800" alt="스크린샷 2024-06-03 오후 4 10 45" src="https://github.com/yapyapHo/sw-ai_business/assets/117447655/7d922807-b19d-4a1a-a304-710847227ec9">
</p>
'시간표 도와줄게유' 서비스는 '시간표 짜기', '학점 계산기', '졸업요건 확인'의 기능을 담고 있습니다. 아래에서 각각의 기능과 사용 방법을 보시면 됩니다. 이 서비스는 알파 버전으로, 아직 시간표 짜기 부분만 구현되었다는 점 말씀드립니다.


</br></br>

# '시간표 짜기' 메뉴
먼저 상단의 시간표 짜기 메뉴를 누르고, 자신의 소속 대학과 전공을 고르시면 됩니다.
<p align="center">
  <img width="350" alt="스크린샷 2024-06-07 오후 2 46 02" src="https://github.com/yapyapHo/sw-ai_business/assets/117447655/891c8686-aab0-4e19-8431-338144a88acd">
</p>
이후 '전공과목 선택하러 가기' 버튼을 누르게 되면, 여러분의 전공의 전공 과목 목록이 뜨게 됩니다.
</br></br>
<p align="center">
  <img width="700" alt="스크린샷 2024-06-07 오후 2 49 23" src="https://github.com/yapyapHo/sw-ai_business/assets/117447655/b3db9b18-a851-4348-a6c3-1b7c6827fa71">
</p>
꼭 들어야 하는 전공 과목들을 선택하시면, 시간표에 나타나게 됩니다. 요일과 시간이 겹치는 경우 선택이 되지 않고 에러가 나니 마음껏 설정하셔도 됩니다.</br></br>
여기서 과목들을 넣으시면 되며, 같은 과목을 한 번 더 누르면 선택 취소되어 시간표에서 지워집니다.</br></br>
<p align="center">
<img width="400" alt="스크린샷 2024-06-07 오후 2 49 41" src="https://github.com/yapyapHo/sw-ai_business/assets/117447655/7ae86f3b-5bd8-4239-a1a0-0bb397a67e6e">
</p>
이 과정을 마치면, 위 사진과 같이 선택하신 전공 과목들이 들어가게 됩니다.</br></br>

이제 원하시는 공강 요일, 팀플 빈도/과제량/학점이 후한 정도 중 여러분이 더 선호하시는 부분을 체크하시면 되고, 과목 추천에 마일리지도 고려하기 위해 여러분의 최대 마일리지도 작성해주시면 됩니다.

여기서 공강 요일은 2개까지만 고를 수 있게 했습니다. 3개 이상 요일을 공강으로 만들기 위한 과목들이 존재하지 않을 수 있는 경우를 방지했습니다.
</br>
<p align="center">
<img width="350" alt="스크린샷 2024-06-07 오후 2 52 24" src="https://github.com/yapyapHo/sw-ai_business/assets/117447655/45736b37-8a08-4e6d-a256-2ec822e82a23">
</p>
'완료!' 버튼을 누르시면, 총 마일리지와 공강 요일, 선호도를 종합해 수강 편람에 있는 과목들을 추천해드립니다.</br></br>
<p align="center">
<img width="700" alt="스크린샷 2024-06-07 오후 2 52 39" src="https://github.com/yapyapHo/sw-ai_business/assets/117447655/9da2ab8b-09d0-4efa-b5f1-6828c3949991">
</p>
여기서도 마찬가지로 같은 과목을 한 번 더 누르면 선택 취소되어 시간표에서 지워집니다.</br></br>
<p align="center">
<img width="400" alt="스크린샷 2024-06-07 오후 2 52 59" src="https://github.com/yapyapHo/sw-ai_business/assets/117447655/4511ca65-eeb7-4b46-b4dd-d129df5c62f0">
</p>
선택을 하시면 위 시간표가 업데이트되는 것을 보실 수 있습니다.</br></br>

여러분의 공강을 사수해보시고, 이 서비스의 존재를 몰라 매일 학교에 헬강 들으러 가야 하는 친구들을 마구 놀려줍시다.</br></br>

# '여러분의 목소리' 메뉴

사용자가 피드백을 할 수 있는 기능입니다. 여러분이 사용하시다 불편하거나 확장 방향성이 생각나신다면 언제든 이용해주세요.
<p align="center">
<img width="400" alt="스크린샷 2024-06-07 오후 3 37 08" src="https://github.com/yapyapHo/sw-ai_business/assets/117447655/754b5fed-ea60-42f2-b5a7-e8c0206198a3">
</p>

유효한 이메일 주소와 피드백을 작성하고 제출하시면, 제게 메세지가 전달됩니다. 피드백은 재빠르게 반영하겠습니다. 감사합니다.</br></br>


# '서비스 소개' 메뉴

구현 내용과 확장 방향성을 소개하고, 사용자가 관심을 가질 만한 요소들을 넣었습니다. 어떤 기능들이 새롭게 추가될지 둘러보세요.</br></br>

# '나의 시간표' 메뉴

시간표 짜기 메뉴에서 완료한 시간표를 불러와 볼 수 있습니다.

구현 예정입니다.</br></br>

# '학점 계산기' 메뉴

에브리타임에 있는 기능이며, 여러분이 받으신 학점을 입력하시면 해당 학기 및 전체 학기 평균 학점을 계산할 수 있습니다.

구현 예정입니다.</br></br>

# '졸업요건 확인' 메뉴

연세포털 내의 졸업요건은 매우 부정확하며 의미가 없습니다. 따라서 여러분이 소속 대학과 전공을 선택하시면 지금까지 들었던 과목들을 종합해 졸업요건을 정확하게 보여드리겠습니다.

구현 예정입니다.
