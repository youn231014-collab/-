# 사계의 모래시계 — 360° 메타버스 공연장

브라우저에서 바로 들어가는 3D 메타버스 공연장입니다. 가운데 모래시계를 중심으로 원형 무대가 봄·여름·가을·겨울 네 구역으로 나뉘어 있고, 플레이어는 브라운/그레이 캐릭터를 골라 무대와 객석을 걸어 다닐 수 있습니다.

## 파일
| 파일 | 설명 |
|---|---|
| `index.html` | 공연장 전체 (Three.js) |
| `chibi.glb` | 플레이어 3D 캐릭터 (Meshy 모델을 6만 폴리곤으로 줄여 텍스처 포함) |
| `chibi_gray.jpg` | 그레이 머리 캐릭터 텍스처 |
| `.github/workflows/pages.yml` | GitHub Pages 자동 배포 |

## 멀티플레이
별도 서버 없이 브라우저끼리 직접 연결합니다 (WebRTC, [Trystero](https://github.com/dmotz/trystero) — 공개 Nostr 릴레이로 서로를 찾음). 같은 주소에 접속한 사람끼리 서로의 캐릭터, 위치, 이름이 실시간으로 보입니다. 이름은 왼쪽 위 패널의 '내 이름' 칸에서 바꿀 수 있습니다.

일부 회사·학교 네트워크처럼 WebRTC를 막는 곳에서는 연결되지 않을 수 있습니다.

## 웹사이트로 켜기 (한 번만)
1. 저장소 **Settings → Pages**
2. **Source** 를 **GitHub Actions** 로 선택
3. **Actions** 탭에서 *Deploy website to GitHub Pages* 를 실행 (또는 새로 푸시)

배포가 끝나면 `https://youn231014-collab.github.io/-/` 에서 열립니다.

## 조작
- 걷기: `W A S D` · 달리기 `Shift` · 점프 `Space` · 드래그로 카메라
- 모래시계 클릭/버튼: 모래시계가 뒤집히며 무대 회전
- `L` 무대 조명 켜기/끄기 · `B` 무빙 빔 켜기/끄기
