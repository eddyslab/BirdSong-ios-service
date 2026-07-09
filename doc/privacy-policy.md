---
canonical: https://eddyslab.github.io/BirdSong-ios-service/privacy-policy.html
meta-description: Privacy for the BirdSong App on iOS App Store
meta-generator: Jekyll v3.10.0
meta-og:description: Privacy for the BirdSong App on iOS App Store
meta-og:locale: en_US
meta-og:site_name: BirdSong-ios-service
meta-og:title: BirdSong 개인정보처리방침 (Privacy Policy)
meta-og:type: website
meta-og:url: https://eddyslab.github.io/BirdSong-ios-service/privacy-policy.html
meta-twitter:card: summary
meta-twitter:title: BirdSong 개인정보처리방침 (Privacy Policy)
meta-viewport: width=device-width, initial-scale=1
title: BirdSong 개인정보처리방침 (Privacy Policy) | BirdSong-ios-service
---

# BirdSong 개인정보처리방침 (Privacy Policy)

**최종 수정일 / Last Updated: 2026-07-09**

---

## 한국어

### 1. 개요

BirdSong(이하 "본 앱")은 eddyslab(이하 "개발자")이 제공하는 음향 기반(GGWave) 메시징 애플리케이션입니다. 본 앱은 오디오/초음파 신호를 통해 기기 간 암호화된 메시지를 전송합니다. 본 개인정보처리방침은 본 앱이 어떤 정보를 처리하는지 설명합니다.

### 2. 수집하는 정보

본 앱은 별도의 회원가입이나 로그인을 요구하지 않으며, 광고 SDK나 분석(Analytics) 도구를 사용하지 않습니다. 아래 정보만 서비스 제공을 위해 처리됩니다.

- **마이크 오디오**: 메시지를 인코딩/디코딩하기 위해 실시간으로 마이크 입력을 처리합니다. 오디오는 녹음되거나 서버에 저장되지 않으며, 신호 처리 즉시 폐기됩니다.
- **메시지 내용 (텍스트/이미지)**: 전송 전 기기에서 AES-256-GCM 방식으로 암호화됩니다. 암호화된 데이터는 단축 URL 코드와 함께 Cloudflare Workers 서버에 일시적으로 저장되며, 약 3분(TTL)이 지나면 자동으로 삭제됩니다.
- **PIN 해시**: 발신자와 수신자 간 페어링 및 메시지 인증을 위해 PIN을 해시 처리하여 사용합니다. 원본 PIN은 서버에 저장되지 않습니다.
- **기기 페어링 정보**: 근거리 기기 간 연결을 위한 최소한의 식별 정보만 일시적으로 사용됩니다.

### 3. 정보 이용 목적

수집된 정보는 오직 다음 목적으로만 사용됩니다.

- 기기 간 암호화된 메시지 전송 및 수신
- 메시지 유효 시간(TTL) 관리
- 앱의 핵심 기능(페어링, 인증) 제공

### 4. 정보 보관 및 삭제

메시지 및 이미지 데이터는 Cloudflare Workers 서버에 암호화된 상태로 일시 저장되며, TTL(약 3분) 경과 시 자동 삭제됩니다. 개발자는 암호화 키를 보유하지 않으므로 서버에 저장된 데이터 내용을 열람할 수 없습니다.

### 5. 제3자 제공

본 앱은 수집된 정보를 제3자에게 판매, 대여, 공유하지 않습니다. 광고 네트워크, 분석 도구, 크래시 리포팅 SDK 등 제3자 서비스를 사용하지 않습니다.

### 6. 데이터 보안

모든 메시지 및 이미지 콘텐츠는 전송 전 AES-256-GCM으로 암호화되며, 키 유도에는 PBKDF2-SHA256이 사용됩니다. 서버는 암호화된 데이터만 일시적으로 중계할 뿐, 복호화 키에 접근할 수 없습니다.

### 7. 필요 권한 (iOS)

- **마이크 (Microphone)**: 오디오 기반 메시지 송수신을 위해 필요합니다. 앱 최초 실행 시 iOS 시스템 권한 요청 팝업을 통해 동의를 받습니다.
- **사진 보관함 / 카메라 (선택)**: 이미지 메시지를 전송하거나 수신한 이미지를 저장하려는 경우에만 사용됩니다.
- **네트워크 접근**: 암호화된 데이터의 단축 URL 업로드/다운로드를 위해 사용됩니다. (별도의 시스템 권한 팝업 없이 자동 허용되는 iOS 표준 동작입니다.)

### 8. 아동의 개인정보

본 앱은 만 13세 미만 아동을 대상으로 하지 않으며, 아동으로부터 고의로 개인정보를 수집하지 않습니다.

### 9. 정책 변경

본 방침은 필요에 따라 개정될 수 있으며, 변경 시 본 페이지를 통해 공지합니다.

### 10. 문의처

개인정보처리방침에 대한 문의사항은 아래 이메일로 연락해 주세요.

**이메일 (Email): dev@eddyslab.com**

---

## English

### 1. Overview

BirdSong ("the App") is an acoustic messaging application developed by eddyslab, using the GGWave library to transmit encrypted messages between devices via audio/ultrasound signals. This Privacy Policy explains what information the App processes.

### 2. Information We Process

The App does not require account registration or login, and does not use advertising SDKs or analytics tools. Only the following information is processed to provide the service:

- **Microphone audio**: Used in real time to encode/decode messages. Audio is not recorded or stored on any server; it is discarded immediately after signal processing.
- **Message content (text/images)**: Encrypted on-device using AES-256-GCM before transmission. Encrypted data is temporarily stored on a Cloudflare Workers server along with a short URL code, and is automatically deleted after approximately 3 minutes (TTL).
- **PIN hash**: A hashed PIN is used for pairing and message authentication between sender and receiver. The original PIN is never stored on the server.
- **Device pairing information**: Minimal identifiers used temporarily to establish a connection between nearby devices.

### 3. Purpose of Use

Information is used solely for:

- Sending and receiving encrypted messages between devices
- Managing message time-to-live (TTL)
- Providing core app functionality (pairing, authentication)

### 4. Data Retention and Deletion

Message and image data are stored temporarily on Cloudflare Workers in encrypted form and are automatically deleted after the TTL (~3 minutes) expires. The developer does not hold decryption keys and cannot view the content of stored data.

### 5. Third-Party Sharing

The App does not sell, rent, or share collected information with third parties. No advertising networks, analytics tools, or crash-reporting SDKs are used.

### 6. Data Security

All message and image content is encrypted using AES-256-GCM prior to transmission, with PBKDF2-SHA256 used for key derivation. The server only relays encrypted data temporarily and has no access to decryption keys.

### 7. Permissions Required (iOS)

- **Microphone**: Required for sending/receiving audio-based messages. Consent is requested via the standard iOS system permission prompt on first use.
- **Photo Library / Camera (optional)**: Used only when sending image messages or saving a received image.
- **Network Access**: Used to upload/download encrypted data via short URLs. This is standard iOS behavior and does not require a separate system permission prompt.

### 8. Children's Privacy

The App is not directed to children under 13, and does not knowingly collect personal information from children.

### 9. Changes to This Policy

This policy may be updated as needed. Changes will be posted on this page.

### 10. Contact

For questions about this Privacy Policy, please contact:

**Email: dev@eddyslab.com**

