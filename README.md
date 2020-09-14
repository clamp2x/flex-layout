# flex-layout
FLEX 레이아웃은 SNAX 스토어에서 판매되는 Slow, Alice, #HASHTAG 등의 다크모드를 지원하는 제품들과 호환되는 무료 오픈소스 레이아웃입니다. 라이믹스 전용으로 제작되었습니다. 다크모드가 범용적으로 사용될 수 있길 바라며, 유료 제품의 일부 소스를 가져와 기초적인 프레임으로 사용할 수 있도록 배포하게 되었습니다. 물론 바로 사용하실 수 있지만 아주 기초적인 레이아웃의 형태만 갖추고 있기 때문에 사용하기 어려울 수 있습니다.

 

> 건전한 피드백은 허용합니다만, 개발할지 말지는 제 선택입니다. 무리한 요구나 사용법에 대한 질문, 기술지원 관련 사항 모두 거부하겠습니다. 개발의 접근성과 오픈소스 품질 향상을 위해 진행하는 프로젝트이니 이 점 꼭 숙지해주세요.

 

GPL 3.0 라이센스를 채택했습니다.
원작자 표기 희망하며, 자유로운 수정, 재배포 환영합니다.

미리보기: https://calvinsnax.com/flex_board/34695


# 다크모드는 어떤식으로 구현되나요?
제가 개발하는 방식은 쿠키를 기반으로 다크모드를 전환합니다. `is_dark_theme`라는 쿠키의 값이 존재할 경우 다크모드로 인식합니다. 현재는 true라는 값을 저장하고 있습니다만, 값의 존재유무로만 판단하도록 개발해두어서 값 자체는 의미가 없습니다. 이 구현 방식은 제 스타일일 뿐이기 때문에 자유로운 토론을 통해 다크모드의 기반 기술을 자유롭게 구현해보시는 것을 추천합니다. 쿠키값의 존재유무를 구분하여 `config.php` 파일에 저장된 scss 변수들을 불러올 때 다크모드에 맞는 변수 값을 가져와 scss 파일에 전달합니다. 길게 말하는 건 의미가 없는 것 같고 `_import.html` 파일을 뜯어보시면 알 수 있습니다.
