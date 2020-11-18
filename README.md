# good_pose /w electron webview

* https://teachablemachine.withgoogle.com/ 에서 학습한 pose classification weight를 사용, electron으로 묶어 실행을 편하게 함.
* 바른 자세가 아닌 프레임이 200개 이상 이어지면 os알림이 뜸! 바른자세 바른정신!
* Using pose classification weight trained on teachable machine site, wrapped with electron.
* if your pose is not good straight 200 frames, os alarm will pop up.
---
* usage : 
    * [teachable machine](https://teachablemachine.withgoogle.com/)에서 바른 자세/바르지 못한 자세 train 
    * weight 받아서 ./my_model에 압축 해제
    * ```electron .``` 로 실행.
---
* todo
    * electron exe로 컴파일 하면 tensorflow.js 불러오는데 에러가 발생함.
    * electron 창이 최소화 되면(~포커스 잃으면) 실행이 멈춤
        * 그냥 브라우저에서 다른 탭 보고 있으면 멈추길래 electron으로 띄우면 괜찮지 않을까 했는데 여전히 문제 발생...
        * browser단의 문제라고는 하는데 조금 더 봐야 함.
        * 일단 창을 항상 위로 띄우게 하여 구동은 확인.


# 참고 : 
- https://github.com/TutorialBook/electron-webview-example
- https://snutiise.github.io/html5-desktop-api/