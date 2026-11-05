# JINWOO KOREA — 임시 미리보기 (Temporary Preview)

> ⚠️ **임시 저장소** — 정식 출시(jnvia.com 배포) 후 삭제 예정입니다.

이 저장소는 **외부에서 임시로 사이트를 확인하기 위한 정적 빌드 산출물**만 담고 있습니다.

- **미리보기 주소**: https://tonykim80.github.io/jinwoo-preview/
- **정식 사이트**: 출시 후 https://jnvia.com (Cloudflare 배포 예정)
- **소스 코드**: private 저장소 `TonyKim80/jinwoo-korea` 에만 있습니다 (여기엔 없음)

## 미리보기 제약 (정상 동작 아님)

| 항목 | 상태 |
| --- | --- |
| 페이지·디자인·이미지·영상·ko/en 전환 | ✅ 실제와 동일 |
| 제품 검색·카테고리 탭·견적 문의 자동입력 | ✅ 실제와 동일 |
| 문의폼·RFQ 첨부 전송 | ❌ 비활성 (안내 토스트 표시) — 정식 배포 후 `sales@jnvia.com` 발송 |
| 공지사항(API 연동) | ❌ 미표시 |
| 검색엔진 색인 | 차단 (`noindex` + robots.txt disallow) — 출시 전 중복 색인 방지 |

## 빌드 방법 (참고)

원본 소스에서 다음을 적용해 `next build` 정적 내보내기(output: export)한 결과물입니다:

- `basePath: /jinwoo-preview`, `images.unoptimized`
- API 라우트 제외 (문의폼·공지 — 정적 호스팅에서 동작 불가)
- robots/noindex 처리 (임시 주소 색인 방지)
