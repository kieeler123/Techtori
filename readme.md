📚 TechTori

React + TypeScript + Vite + Tailwind / Node.js + Express / MongoDB Atlas

🇰🇷 한국어 (Korean)
🚀 개요

TechTori는 개발 관련 글·링크를 저장하고, 검색하고, 정리할 수 있는 미니 블로그/북마크 앱입니다.
검색, 태그 필터, 날짜 필터, 페이지네이션, UI 상태 복원(localStorage) 등을 지원합니다.

🛠 기술 스택
레이어 기술
프론트엔드 React, TypeScript, Vite, TailwindCSS, Axios
백엔드 Node.js, Express
데이터베이스 MongoDB Atlas, Mongoose
✨ 주요 기능

글/링크 생성 · 조회 · 삭제

텍스트 검색($text) + 정규식 보조 검색

태그 AND 필터링

날짜 범위(from–to) 필터

최신순/과거순 정렬

페이지네이션

localStorage 기반 UI 상태 자동 복원

API 표준 응답 구조: { data, total, page, pages }

🔧 설치 및 실행

1. 서버
   cd server
   npm install
   npm run dev # http://localhost:4000

server/.env

MONGO_URI=mongodb://localhost:27017/techtori
PORT=4000
CLIENT_URL=http://localhost:5173

2. 클라이언트
   cd client
   npm install
   npm run dev # http://localhost:5173

client/.env

VITE_API_BASE=http://localhost:4000

📁 폴더 구조
client/
├─ components/
├─ hooks/
├─ services/ # axios 인스턴스
└─ types/

server/
├─ controllers/
├─ models/
├─ routes/
└─ server.ts

☁️ 배포

백엔드: Render

MONGO_URI, CLIENT_URL 설정

코드 변경 → Git 푸시 시 자동 배포

환경변수 변경 → 콘솔 수정 후 수동 재배포

프론트: Vercel

VITE_API_BASE=https://<server-url>

env 수정 시 반드시 재배포 필요

<br><br>

🇯🇵 日本語 (Japanese)
🚀 概要

TechTori は、プログラミング関連の記事やリンクを保存・検索・管理できるミニブログアプリです。
検索、タグ AND フィルタ、日付範囲、ページネーション、localStorage による UI 復元をサポートしています。

🛠 使用技術
レイヤー 技術
フロントエンド React, TypeScript, Vite, TailwindCSS, Axios
バックエンド Node.js, Express
データベース MongoDB Atlas, Mongoose
✨ 主な機能

記事/リンクの作成・取得・削除

$text 検索 + 正規表現によるフォールバック検索

タグの AND フィルタ

日付範囲フィルタリング

昇順/降順ソート

ページネーション

localStorage による UI 状態復元

API レスポンス形式を { data, total, page, pages } に統一

🔧 セットアップ

1. サーバー
   cd server
   npm install
   npm run dev # http://localhost:4000

server/.env

MONGO_URI=mongodb://localhost:27017/techtori
PORT=4000
CLIENT_URL=http://localhost:5173

2. クライアント
   cd client
   npm install
   npm run dev # http://localhost:5173

client/.env

VITE_API_BASE=http://localhost:4000

📁 フォルダ構成
client/
├─ components/
├─ hooks/
├─ services/
└─ types/

server/
├─ controllers/
├─ models/
├─ routes/
└─ server.ts

☁️ デプロイ

バックエンド：Render

MONGO_URI, CLIENT_URL を設定

コード変更 → GitHub 経由で自動デプロイ

環境変数変更 → コンソールで変更後、手動デプロイ

フロントエンド：Vercel

VITE_API_BASE=https://<server-url>

env 変更後は必ず再デプロイ

<br><br>

🇺🇸 English (영문 버전)
🚀 Overview

TechTori is a mini tech-blog/link management app for storing, browsing, and searching programming-related content.
It supports search, tag filtering, date range filtering, pagination, and UI persistence via localStorage.

🛠 Tech Stack
Layer Technologies
Frontend React, TypeScript, Vite, TailwindCSS, Axios
Backend Node.js, Express
Database MongoDB Atlas, Mongoose
✨ Features

Create / list / delete entries

Text search using $text + regex fallback

AND-based tag filtering

Date range filtering

Asc/desc sorting

Pagination

UI state restored from localStorage

Standard API response { data, total, page, pages }

🔧 Setup

1. Server
   cd server
   npm install
   npm run dev # http://localhost:4000

server/.env

MONGO_URI=mongodb://localhost:27017/techtori
PORT=4000
CLIENT_URL=http://localhost:5173

2. Client
   cd client
   npm install
   npm run dev # http://localhost:5173

client/.env

VITE_API_BASE=http://localhost:4000

📁 Project Structure
client/
├─ components/
├─ hooks/
├─ services/
└─ types/

server/
├─ controllers/
├─ models/
├─ routes/
└─ server.ts

☁️ Deployment

Backend: Render

Set MONGO_URI, CLIENT_URL

Code changes → auto-deployed via Git push

Env changes → manual redeploy required

Frontend: Vercel

Set VITE_API_BASE=https://<server-url>

Redeploy required after modifying env variables
