---
layout: post
title:  "Git과 Github"
date:   2022-11-17 17:27:19 +0900
categories: jekyll update
comments : True
---
Git은 로컬 파일의 변경사항을 기록하고 해당 파일에 대한 여러 사용자 간의 작업을 조율하기 위한 버전 관리 시스템(VCS : Version Control System)이다.

Git hub는 깃을 클라우드 방식으로 구현된 버전 관리 시스템(VSC)이다. 로컬 파일을 깃허브 클라우드에 Push(업로드)하여 서로 다른 위치에 있는 여러 사용자가 작업할 수 있다.

방금 Push(업로드)한다고 하였는데 이에 대해 더욱 자세히 다뤄보겠다.

로컬 파일의 변경사항을 원격 저장소에도 적용시키기 위해서 git에선 add-commit-push 과정을 거친다.

먼저 git add [파일이름]을 통해 커밋 전에 변경사항들을 Staging Area에 모아둔다.

이후 git commit -m [커밋에 대한 설명]을 통해 변경사항들을 확정 짓고 로컬 저장소에 등록한다.

마지막으로 git push 명령어를 통해 로컬저장소에 등록된 변경사항을 원격저장소에도 적용시킨다.

반대로 git pull은 원격저장소에서의 변경사항을 로컬저장소에 적용시킬 때 사용한다.

이처럼 git과 github은 협업할 때 자주 사용되므로 잘 숙지해두는게 좋다.







