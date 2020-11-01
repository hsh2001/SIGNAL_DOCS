## Naver AD (WIP)

### [RelKwdStat: list](https://naver.github.io/searchad-apidoc/#/operations/GET/~2Fkeywordstool)

#### Request

- hintKeywords: 힌트를 얻기 위한 키워드 리스트입니다. 리스트 내 아이템간 구분자로는 컴마를 사용하며 (예: 꽃배달,flower,화환,bouquet), 최대 5개 키워드까지 리스트에 넣을 수 있습니다.
- showDetail: 각각 연관어마다 자세한 통계 정보 (쿼리량, 클릭량, 클릭률, 경쟁 지수, 광고 갯수)를 얻으려면 `showDetail = 1`로 설정하세요. 연관어와 매달 쿼리량 정보만 얻어오려면 `showDetail = 0`로 설정하세요.

#### Response

아래 응답 값은 항상 배열로 리턴합니다.

- relKeyword: 연관 검색어
- monthlyPcQcCnt: PC 쿼리량
- monthlyMobileQcCnt: 모바일 쿼리량
- monthlyAvePcClkCnt: PC 클릭수 (`showDetail = 1`인 경우)
- monthlyAveMobileClkCnt: 모바일 클릭수 (`showDetail = 1`인 경우)
- monthlyAvePcCtr: PC 클릭률 (`showDetail = 1`인 경우)
- monthlyAveMobileCtr: 모바일 클릭률 (`showDetail = 1`인 경우)
- plAvgDepth: 광고 갯수 (`showDetail = 1`인 경우)
- compIdx: 광고 경쟁 지수 (`showDetail = 1`인 경우)
