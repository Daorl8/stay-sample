# STRUCTURE — stay-sample (GOYO)

단일 페이지(`index.html`). **서사-퍼스트 롱스크롤** + **풀블리드 교차** 레이아웃 + 스티키 상단 내비. 다크 팔레트.

```
index.html
├─ <head> : 메타, 폰트(Cormorant Garamond + Pretendard), 인라인 CSS(다크 토큰)
├─ .topnav (sticky, 투명→스크롤 시 솔리드) — 브랜드 + 앵커 + 예약 CTA
├─ #hero       Hero : 풀블리드 다크 + 선언문 헤드라인 1줄 + 스크롤 큐
├─ #prologue   Prologue : 짧은 서사 카피(공간보다 '밤'을 판다)
├─ #space      The Space : 풀블리드 교차(침실/거실/욕실/테라스) — 이미지 풀블리드 + 오프셋 텍스트 교대
├─ #night      A Night Here : 체크인→저녁→아침 경험 서사
├─ #details    Details : 객실 정보·정원·포함사항·가격 (실용 정보는 *일부러 뒤에*)
├─ #reserve    Reservation : 예약 문의 폼 + 네이버 예약 버튼
├─ #location   Location : OSM 지도 + 길찾기·전화
├─ 모바일 하단 퀵바 (.mbar, <div>) : 전화 / 예약 문의
└─ <script> : 스티키 내비 솔리드 토글(rAF), 데스크탑 전용 리빌, 폼
```

## 디자인 토큰
- 컬러: `--bg:#14130F` `--surface:#1E1C17` `--text:#EDE7DB` `--muted:#A29C8C` `--gold:#B89160` `--line:#33302A`
- 타입: 헤드라인 `Cormorant Garamond`(라이트), 본문 `Pretendard`. 한/영 병기.
- 모션: 데스크탑 스크롤 페이드/슬라이드(≥861px), 모바일 정적. `word-break:keep-all`.
