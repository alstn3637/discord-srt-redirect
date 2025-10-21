# Discord SRT Bot Dashboard Redirect

이 페이지는 VS Code Tunnel URL이 변경되어도 고정된 URL로 대시보드에 접속할 수 있도록 자동 리다이렉트를 제공합니다.

## 🌐 고정 접속 URL
```
https://[YOUR_USERNAME].github.io/discord-srt-redirect/
```

## 📋 기능
- VS Code Tunnel URL 자동 리다이렉트
- 최신 대시보드 URL 자동 연결
- URL 변경 시에도 동일한 주소로 접속 가능

## 🔄 URL 업데이트 방법

### 방법 1: Python 스크립트 사용
```bash
cd C:\study\discord_srtgo
python update_tunnel_url.py
```

### 방법 2: 수동 업데이트
`tunnel-config.json` 파일을 직접 수정:
```json
{
    "dashboard_url": "새로운 URL",
    "last_updated": "업데이트 시간"
}
```

## 📝 설정 파일
- `index.html`: 리다이렉트 페이지
- `tunnel-config.json`: URL 설정 파일
- `update_tunnel_url.py`: URL 업데이트 스크립트

## 🚀 자동 업데이트
URL이 변경되면:
1. `update_tunnel_url.py` 실행
2. 새 URL 입력
3. Git push
4. GitHub Pages가 자동으로 업데이트

---
Generated with [VS Code Tunnel Auto-Redirect](https://github.com/YOUR_USERNAME/discord-srt-redirect)