# 깃허브(GitHub)에 프로젝트 올리는 방법

현재 프로젝트 폴더에 **로컬 Git 저장소 설정(git init, commit)**까지는 제가 완료했습니다.
이제 깃허브 웹사이트에서 저장소를 만들고 연결만 하시면 됩니다.

### 1단계: 깃허브 저장소 생성
1. [GitHub](https://github.com)에 로그인합니다.
2. 우측 상단의 `+` 버튼을 누르고 **New repository**를 클릭합니다.
3. **Repository name**에 프로젝트 이름(예: `5-days-brain-game`)을 입력합니다.
4. **Public**(공개) 또는 **Private**(비공개)를 선택합니다.
5. **Create repository** 버튼을 클릭합니다.

### 2단계: 내 컴퓨터와 연결하기
저장소가 생성되면 화면에 나오는 명령어 중 **"…or push an existing repository from the command line"** 부분의 코드를 복사해서 터미널에 입력해야 합니다.

터미널을 열고 아래 명령어들을 순서대로 입력하세요 (복사해서 붙여넣기):

```bash
# 1. 깃허브 저장소 주소 연결 (YOUR_USERNAME은 본인 아이디로 변경)
git remote add origin https://github.com/YOUR_USERNAME/5-days-brain-game.git

# 2. 메인 브랜치 이름 변경 (보통 main 사용)
git branch -M main

# 3. 깃허브로 코드 올리기
git push -u origin main
```

### 3단계: 배포 (선택사항)
코드를 올린 후, 이 게임을 웹에서 다른 사람들이 할 수 있게 하려면 **Vercel**이나 **GitHub Pages**를 이용할 수 있습니다.

**Vercel 배포 (가장 추천):**
1. [Vercel](https://vercel.com) 회원가입 (GitHub 아이디로 로그인)
2. **Add New...** -> **Project** 클릭
3. 방금 올린 GitHub 저장소(`5-days-brain-game`)를 Import
4. **Deploy** 클릭하면 끝! (자동으로 링크가 생성됩니다)
