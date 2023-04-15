

23.04.14

 
CLI branch & conflict 실습을 위한 manual directory 생성

work.txt를 이용하여 apple, ms, google 등 여러가지 브런치를 생성
checkout을 통해 브런치를 이동하였을 때 변화 확인.

23.04.15

manual-merge directory 생성

work.txt 라는 파일을 다른 branch에서 수정 후 병합

다른 부분을 수정한 뒤 병합하였을 때 git이 알아서 수정해서 병합해줌.

같은 부분을 수정한 뒤 병합하였을 때 conflict 발생.
git이 자동으로 병합해 주지않음. 해당 부분에 대한 수정을 하여햐 병합해줌.


- 3 way merge 

here   base   there    2way_merge    3way_merge
 A      A       A          A             A
 H      B       B          ?             H
 C      C       T          ?             T
 H      D       T          ?             ?


here , there : branch
base : branch가 쪼개져 나갈 때의 공통의 조상 
2 way merge 에서는 충돌이 일어날 때, 직접 해결해야 하는 부분이 3가지임.
3 way merge 에서는 공통의 조상인 base와 비교함으로써 어떤 부분이 수정됬는지 알기 용이함.
수정된 부분을 자동으로 확인하여서 직접 해결해야하는 부분을 줄일 수 있음.


-mergetool 을 이용한 병합

mergetool로 vscode를 이용하여 보다 시각적으로 conflict 부분 해결가능.



