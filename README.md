# LifeSelect Profile Link MVP

정적 파일 2개만으로 동작합니다.

- index.html
- products.json

## 실행
로컬에서 단순히 파일을 더블클릭하면 브라우저의 CORS 정책 때문에 products.json 로딩이 막힐 수 있습니다.
아래처럼 간단한 로컬 서버를 띄우세요.

python -m http.server 8000

그 다음:
http://localhost:8000

## 제품 추가
products.json에 객체 하나를 추가하면 됩니다.

{
  "id": "unique-id",
  "title": "제품명",
  "category": "주방",
  "description": "한 줄 설명",
  "url": "https://naver.me/...",
  "emoji": "🛍️"
}

## 배포
GitHub Pages, Vercel, Netlify 등 정적 호스팅 어디든 바로 올릴 수 있습니다.
