# Deep-Learning-Lecture
[1. tasks_190730.py]

tensorflow 등을 사용하지 않고 Apporximeter (사용하고자 하는 모델)을 fx = ax^2 + bx + c의 이차방정식으로 설정.
주어진 X, Y값을 가지고 weight를 최적화스럽게 찾아가는 코드이다.

참고로 weight를 갱신할 때, 
W = W - learning late * E'(w) 
--> E'(w)는 (y-f(x))^2의 sum을 최소화하는 것으로, (1) (y-f(x))^2한고 모두 더한 후 미분하는 방식보다 (2) (y-f(x))^2을 합성미분하 것을 모두 더한 것은 동일하며 (2)방식으로 코딩하면 X, Y 개수가 변동이 있어도 소스를 변경할 필요가 없다.

