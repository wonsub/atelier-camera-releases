# Atelier Camera

Android용 Atelier 무선 버추얼 카메라 앱의 테스트 배포입니다. 최신 버전은 **0.2.0**입니다. 기존 앱을 삭제하지 말고 APK를 열어 업데이트 설치하세요.

**[APK 다운로드](https://github.com/wonsub/atelier-camera-releases/releases/latest/download/atelier-camera.apk)**

1. Android 8 이상에서 APK를 내려받아 설치합니다. 브라우저의 앱 설치 허용이 필요할 수 있습니다.
2. 외부에서 연결하려면 PC와 휴대폰의 [Tailscale](https://tailscale.com/download/android)을 같은 계정으로 연결합니다.
3. PC에서 `Start-Atelier.bat` 실행 → **스마트폰 카메라** → **무선 페어링 시작**.
4. 앱의 **연결 → PC 페어링 QR 스캔**로 PC에 표시된 페어링 QR을 스캔합니다. 다운로드 QR과 페어링 QR은 서로 다릅니다.
5. **메뉴 → 6DoF 추적 시작** 또는 **3DoF 추적 시작** → PC 프리뷰 확인 → **REC** → **정지**.

6DoF는 ARCore 지원 기기와 Google Play Services for AR가 필요합니다. 3DoF는 회전만 측정합니다. 휴대폰 실제 하드웨어 추적 정확도는 아직 검증하지 않았습니다.

연결은 사설 Wi-Fi 또는 Tailscale IPv4 HTTPS/WSS이며, QR의 인증서 지문으로 PC를 확인합니다. 공용 인터넷에 PC 포트를 개방할 필요가 없습니다. PC 스튜디오는 켜져 있어야 하며 연결 설정창은 닫아도 됩니다. 메인 뷰의 카메라 바에서 LIVE/REC를 조작하고, 씬 편집·저장은 라이브 일시정지 후 진행하세요. 앱은 공개 다운로드할 수 있지만, 제어하려면 자신의 PC가 발급한 페어링 QR이 필요합니다.

원본은 휴대폰 앱 내부에 보관되며 **보관한 원본**에서 PC 재전송과 JSON 공유가 가능합니다. 앱 삭제 시 내부 원본도 삭제됩니다. 중요한 원본은 별도로 내보내세요. PC를 종료하기 전에 씬을 저장하세요.

[개인정보 안내](PRIVACY.md) · [사용 라이브러리](THIRD_PARTY_NOTICES.md)

0.2.0: 전체 화면 프리뷰, 가로 화면의 측면 조작부, 화면만/조작 표시 전환, 접힌 연결·추적·보관 메뉴를 제공합니다. 세로·가로 회전 시 프리뷰 뷰를 유지합니다.

