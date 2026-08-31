# 현금출납부 (Cashbook)

Google Sheets 현금출납부를 웹으로 구현한 경량 앱.

## 구조

```
├── index.html          # 프론트엔드 (Vercel 배포)
├── style.css
├── vercel.json
└── backend/            # FastAPI 백엔드
    ├── main.py
    ├── models.py
    ├── storage.py
    ├── auth.py
    └── requirements.txt
```

## 배포

- **프론트엔드**: Vercel (`mini-cashbook.vercel.app`)
- **백엔드**: DEVFORGE 서버 (port 8100)

## 백엔드 실행

```bash
cd backend
pip install -r requirements.txt
CASHBOOK_API_KEY=your-key python3 -m uvicorn main:app --host 0.0.0.0 --port 8100
```

## 접속

1. 앱 접속 → 서버 주소 + API 키 입력
2. 서버 주소: `https://devforge.152-69-229-246.nip.io/cashbook`
3. API 키: `CASHBOOK_API_KEY` 환경변수 값
