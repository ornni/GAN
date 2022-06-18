CGAN을 이해하기 위해서는 GAN과 Loss Function을 비교하여 살펴보면 빠르게 이해할 수 있다.<br/>

Loss Function

GAN

![GAN Loss Function](https://github.com/ornni/GAN/blob/main/CGAN/image/GAN%20Loss%20Function.png?raw=true)

CGAN

![CGAN Loss Function](https://github.com/ornni/GAN/blob/main/CGAN/image/CGAN%20Loss%20Function.png?raw=true)

기존의 GAN은 noise z를 갖고 무작위로 이미지를 생성했지만, CGAN의 경우 특정 레이블 y가 추가되면서 특정한 이미지를 고정적으로 생성<br>

(GAN모델에서 생성되는 이미지를 마음대로 조절할 수 없다는 문제를 해결하며 z가 원하는 방향으로 이미지를 생성하도록 만듦)<br>

ex) MNIST 데이터에서 7에 해당하는 데이터만 사용하도록 설정<br>

한계: MNIST 데이터의 경우 y의 값이 0~9까지의 class이기 때문에 이미지를 생성하는 것은 어렵지 않지만, 현실적으론 복잡한 이미지들은 변수가 매우 많음
