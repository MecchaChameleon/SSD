# privacy → SSD 저장소 전환 안내

기존 `MecchaChameleon/privacy` 저장소의 이름은 `MecchaChameleon/SSD`로 변경되었습니다. 이 로컬 폴더도 `https://github.com/MecchaChameleon/SSD.git`에 연결했고, 로컬 `main`이 원격 `origin/main`을 추적하도록 설정했습니다. 작성한 README·docs·assets는 아직 커밋하거나 push하지 않은 상태입니다.

## 기존 파일 보존

`index.html`은 기존 privacy 저장소에서 가져온 개인정보처리방침 원문입니다. 프로젝트 소개는 `README.md`에 두고, 개인정보처리방침 파일은 기존 위치에 유지합니다. 개인정보처리방침의 문구는 이번 정리에서 변경하지 않았습니다.

## 이름 변경 전 확인

GitHub 저장소 이름을 바꾸면 저장소 링크와 Git 접근은 새 이름으로 연결되지만, GitHub Pages의 프로젝트 사이트 주소는 자동으로 리다이렉트되지 않습니다.

Pages 기본 주소를 사용 중인 경우 확인할 주소는 다음과 같습니다. 실제 사용 여부와 배포 설정은 GitHub의 Settings → Pages에서 확인합니다.

| 구분 | 주소 |
|---|---|
| 변경 전 기본 주소 | `https://mecchachameleon.github.io/privacy/` |
| 변경 후 기본 주소 | `https://mecchachameleon.github.io/SSD/` |

카카오 개발자 설정, 앱 배포·스토어 설정, 소개 페이지 등에서 개인정보처리방침 URL을 참조한다면 새 주소로 갱신해야 합니다. 확인한 로컬 프론트엔드·백엔드 소스에서는 `github.io` 또는 `privacy` 주소 참조를 찾지 못했으며, 외부 콘솔의 등록값은 별도로 확인해야 합니다.

공식 안내: [GitHub 저장소 이름 변경](https://docs.github.com/en/repositories/creating-and-managing-repositories/renaming-a-repository).

## 전환 순서

1. 기존 privacy 저장소의 Settings → General에서 Repository name을 `SSD`로 변경합니다.
2. 이름을 변경한 기존 저장소를 clone하거나, 기존 clone의 origin을 새 주소로 바꿉니다.
3. 이 폴더의 README, docs, assets를 기존 저장소에 추가합니다. `index.html`은 동일 원문을 유지합니다.
4. 기존 커밋 이력이 있는 저장소에서 변경사항을 커밋하고 push합니다.
5. GitHub Pages를 사용 중이면 새 주소에서 개인정보처리방침이 열리는지 확인하고 외부 등록 URL을 갱신합니다.
6. 조직 프로필에서 SSD 저장소를 고정하면 대표 소개로 접근하기 쉽습니다.

이 로컬 폴더는 기존 privacy 저장소의 커밋 이력을 받아 그대로 이어서 사용합니다. 원격의 기존 개인정보처리방침과 로컬 `index.html`도 동일합니다.

## 데모 영상 표시

현재 README는 `assets/videos/demo.gif`를 이미지로 바로 표시합니다. GIF는 전체 시연을 반복 재생하며, 음성을 포함한 원본은 `assets/videos/demo.mp4`의 상대경로 링크로 제공합니다. MP4는 약 24.6 MiB이며, 원본을 그대로 복사했습니다.

GitHub README 안에서 바로 재생되는 첨부 영상을 원한다면 GitHub의 영상 첨부 URL로 교체하거나, 외부 영상 서비스에 올린 주소를 사용할 수 있습니다. GitHub 영상 첨부 제한은 무료 플랜 10MB, 유료 플랜 100MB이므로 현재 원본은 무료 플랜 첨부 한도를 넘습니다. 이 제한은 저장소에 파일을 커밋하는 경우와 별개입니다.

공식 안내: [GitHub 파일 첨부](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/attaching-files).
