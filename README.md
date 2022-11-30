1. 사전조사

본격적인 블로그 만들기 활동에 앞서, git과 github 그리고 마크다운 언어에 대해 조금씩 공부했다. 

2. 원격저장소 생성

이후 blog를 구성하는 근간이 되는 원격 저장소 Github에 jangjaewoong.github.io라는 이름에 저장소를 만들었다.
이후 배경화면에 blog라는 폴더를 생성하고(폴더 안에 클론하지 않으면 이후 작업에서 오류가 떴음.) 이후 명령 프롬프트에서 작업 디렉토리를 blog로 옮기고 git clone [원격저장소 주소]를 입력해 원격저장소에 있는 파일과 구성요소들을 내 노트북, 즉 로컬저장소에 불러 왔다. 이후 간단한 html을 제작하고, 내 clone한 폴더 내에 추가한다. add-commit-push 과정을 통해 원격저장소에 올리고, 주소창에 저장소 이름(jangjaewoong.github.io)를 입력해 작동이 잘 되는지 확인했다. 

3. Jekyll과 Ruby설치 후 Jekyll 테마 반영

이후 블로그에 테마를 적용하기 위해 Jekyll을 설치해야했는데, window이용자는 Ruby가 필요해서 먼저 Ruby를 설치해줬다. 미리 설치해 둔 git bash에서 원격저장소가 존재하는 디렉토리로 이동한 후에 jekyll을 설치해 줬다. 이후 Jekyll serve 명령어로 내 로컬 주소로 생성된 Jekyll 기본테마의 블로그를 확인 했다. config파일의 블로그 구성요소를 변경해보고 블로그 제작에 감을 잡았다. 이후 원격저장소에 add-commmit-push하여 원격저장소에도 반영할 수 있게 했다. post폴더에 markdown 언어를 이용해 여러 게시물을 작성해보고 블로그에 반영 되는지 확인해보았다.

4. Lanyon 테마 적용

이후 Jekyll 기본 테마 외 새로운 테마를 적용시키기 위해 깔끔한 Lanyon 테마를 골랐다. github에 올라와있는 Lanyon 테마의 구성요소를 git clone을 이용해 로컬 저장소에 받아왔다. 원래 있던 것과 겹치는 파일은 Lanyon의 파일로 덮어쓰기 했다. 그 과정에서 "Bundler could not find compatible versions for gem 'hashie'"이란 오류가 발생하여 bundle update, bundle install 명령어를 통해 해결하였다.

5. 코멘트 기능 구현

마지막으로 코멘트 작성 기능을 구현해보려 했다. 먼저 Disqus 홈페이지의 도움을 받기로 했다. 홈페이지 내의 여러 설정들을 마치고 블로그 속성을 관리하는 파일인 _config.yml에서 disqus를 반영해주었다. 이후 형식관련 파일인 _layouts/post.html에서 disqus형식을 반영해준다. src변수에 내 disqus URL이 확실하게 입력됬는지 조심해야한다. 이후 내가 올리는 post파일에 comments: true를 입력해 코멘트 작성 기능을 불러올 것이라고 입력해준다. 이후 add-commit-push로 원격저장소에 저장해준 뒤 결과를 확인해 줬다.