# USB Debugging

안드로이드에서 개발자모드를 하게되면
특정 명령어나 디버깅을 할 때 USB디버깅에 대한 키를 허용하도록 물어보게된다.
그러나 boot.img를 아래와 같이 수정하게 되면

![bootimg.PNG](/Image/bootimg.PNG)

디버깅을 허용하겠냐는 다이얼로그가 뜨지 않는다.<br>
위와 같은 설정을 하게 되면 모든 USB 경로에서 Authorized가 되어야 한다는데<br>
cmd를켜서 확인해보면 인증되어있지 않다... 왜그런지 이유를 아직은 모르겠다.<br>

따라서 미리 디버깅 허용을 해놓은 컴퓨터에서만 저 설정을 하도록 한다.