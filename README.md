# Blockchain & Full Stack Developer

[![GitHub Stats](https://github-readme-stats.vercel.app/api?username=fdongfdong&show_icons=true&theme=tokyonight&hide_border=true)](https://github.com/fdongfdong)
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=fdongfdong&layout=compact&theme=tokyonight&hide_border=true)](https://github.com/fdongfdong)

EVM 스마트 컨트랙트 설계 · EIP-712 배치 서명 · Foundry TDD | Web3 풀스택

---

## Tech Stack

### Blockchain
![Solidity](https://img.shields.io/badge/Solidity-363636?style=for-the-badge&logo=solidity&logoColor=white)
![Foundry](https://img.shields.io/badge/Foundry-000000?style=for-the-badge&logo=ethereum&logoColor=white)
![Wagmi](https://img.shields.io/badge/Wagmi-1C1B1B?style=for-the-badge&logo=ethereum&logoColor=white)
![Web3](https://img.shields.io/badge/Web3.js-F16822?style=for-the-badge&logo=web3.js&logoColor=white)

### Frontend
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)

### Backend
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)

---

## Projects

### Starlight Passkey Wallet - WebAuthn 기반 암호화폐 지갑

**Web3 Frontend**

WebAuthn PRF를 활용한 제로널리지 패스키 지갑 (생체인식 기반 트랜잭션 서명)

**핵심 기여**
메타마스크 비동기 팝업 UX 문제 해결 → 생체인식 원클릭 서명으로 사용성 개선

**개발 방법론**
`WebAuthn PRF Extension` `AES-GCM Encryption` `HMAC Integrity Verification`

**Tech Stack**
`React 19` `TypeScript` `Viem` `WebAuthn` `BIP39` `HD Wallet`

[![Live Service](https://img.shields.io/badge/Live_Service-4A5AFF?style=for-the-badge&logo=google-chrome&logoColor=white)](https://app.starlightchain.xyz/)

**구현 기능**
- WebAuthn PRF로 암호화 키 생성 (생체인식 기반)
- AES-GCM + HMAC-SHA256 무결성 검증
- 메타마스크 대비 빠른 트랜잭션 서명 (비동기 팝업 제거)
- Multi-chain 지원 (BSC, ETH 등 EVM 호환)

### ERC Token Standards Implementation

**Blockchain**

다양한 ERC 표준을 준수하는 스마트 컨트랙트 설계 및 BSC 메인넷 배포

**구현 표준**
`ERC-20` `ERC-20 Permit` `ERC-721` `ERC-1155`

**Tech Stack**
`Solidity` `Foundry` `Wagmi` `BSC Network`

[![Deployed Contract](https://img.shields.io/badge/BSCScan-FCC624?style=for-the-badge&logo=binance&logoColor=black)](https://bscscan.com/address/0x01B425FDE4653b630e911159FBDb0DB9E41E3dcf)

### Celebus Contracts
**Blockchain** | **Full Stack**

EIP-712 배치 서명 기반 투표·부스팅 시스템 — 100명의 투표를 1건의 트랜잭션으로 처리하여 가스비 70-80% 절감

**핵심 기능**
- EIP-712 구조화 서명 + 2단계 검증 (Executor 배치 + 사용자 개별 서명)
- Soft-fail 배치 처리 — 한 유저의 실패가 전체 배치에 영향 없음
- EOA + 스마트 월렛(ERC-1271) 이중 서명 지원
- 285개 Foundry 테스트 (유닛 + 인배리언트) 전수 통과
- 컨트랙트 인터랙션 대시보드 — 배치 서명·검증 플로우를 시각화하는 Next.js 16 프론트엔드

**설계 방법론**
`EIP-712` `Batch Processing` `Gas Optimization` `Soft-fail Pattern` `Foundry TDD`

**Tech Stack**
`Solidity 0.8.27` `Foundry` `OpenZeppelin 5.x` `Next.js 16` `TypeScript` `viem` `Tailwind CSS v4`

[![View Code](https://img.shields.io/badge/View_Code-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/FDongFDong/celebus-contracts)

---

## Side Projects

### TruthLens - AI 텍스트 검증 서비스

**Full Stack**

한국어 텍스트의 AI 작성 확률을 분석하고 개선 제안을 제공하는 웹 애플리케이션

**개발 방법론**
`Domain-Driven Design` `RESTful API`

**Tech Stack**
`React 18` `TypeScript` `TanStack Router` `Tailwind CSS` `Zustand` `Node.js`

[![View Code](https://img.shields.io/badge/View_Code-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/FDongFDong/truthlens)

### 비디오 다운로더 & 프레임 추출 툴

**Full Stack**

2GB+ 대용량 파일 스트리밍 지원하는 비디오 다운로드 및 프레임 추출 웹 애플리케이션

**핵심 기능**
- 자동/고급 모드 비디오 다운로드 (yt-dlp 기반 1440p60 지원)
- 범용 다운로드 (1000+ 사이트, 쿠키 인증, Chrome 클로닝)
- FFmpeg 프레임 추출 (설정 가능한 FPS, ZIP 압축)
- 2GB+ 파일 스트리밍 (메모리 최적화, ReadStream 방식)
- 실시간 진행률 추적 (sessionId 기반 polling)

**개발 방법론**
`RESTful API` `Session Management` `File Streaming` `Browser Cloning`

**Tech Stack**
`Next.js 15` `React 19` `TypeScript` `Tailwind CSS v4` `yt-dlp` `FFmpeg` `Archiver`

[![View Code](https://img.shields.io/badge/View_Code-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/FDongFDong/downloader)

---

## Learning & Practice

<details>
<summary><b>Click to expand</b></summary>

### Language Practice
- [Go Language](https://github.com/FDongFDong/go_language_practice)
- [TypeScript](https://github.com/FDongFDong/typescript_practice)
- [React.js](https://github.com/FdongFdong/react_practice)
- [Solidity](https://github.com/FDongFDong/solidity_practice)

### Blockchain Study
- [Blockchain Fundamentals](https://github.com/FDongFDong/BlockChain_study)
- [Blockchain Daemon Server](https://github.com/FDongFDong/blockchain_daemon_server)
- [Web3 Practice](https://github.com/FDongFDong/web3-practice)

</details>

---

## Contact

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/FDongFDong)
