# Rooting Order

화면상으로 보이는 루팅의 순서는 다음과 같다.
```
1. /system, /vendor, /data, rootfs를 마운트한다.
2. 인스톨 파일을 추출하고 시스템 안정성을 검사한다.
3. 부트이미지를 생성하고, 마운트하고, 패스를 설정한다.
4. 이전파일을 삭제하고, 파일을 교체한다.
5. 부트이미지를 패치한다.
6. /system, /vendor를 언마운트 한다.
```
과정을 짧게 서술해 보았는데, 실제 실행되는 내부를 살펴보니 쉘 스크립트로 되어있어서 이해하기가 난해하다.<br>

![1](/Image/rooting_order_2.PNG)

![2](/Image/rooting_order_1.PNG)

이해하기위해선 쉘스크립트에 대한 이해와 첫줄부터 천천히 읽어봐야 할 것 같다...