# 5주차 강의 요약
state 
----
state란 system의 내부 상태인 것으로 system에서 나오는 수식에 의미를 부여할 수 있다. state 왜 나오게 되었나면 어떠한 물리적 현상을 수학적 모델로써 system을 계산할 때 직접 또는 컴퓨터가 계산을 해야되게 된다. 이때 조금 더 간단하고 효율적으로 해결하기 위해 쳬계화가 필요해지는데 그래서 state를 사용하게 되었다. 
### state의 장점
----
* 미분 방정식의 차수가 낮아진다.
> 다차 미분 방정식을 1차 미분 방정식의 연립으로 변환이 가능해진다. 예를 들면 2차 미분 방정식은 state를 사용함으로써 1차 미분방정식 2개를 연립한 형태가 되게 된다. 그렇기 때문에 2차 보다는 1차 미분방정식이 문제 풀이나 계산에 용이하므로 쉽게 계산이 가능하다.
* 수식의 해석에 용이해진다.
> 위에서 말했듯 state를 사용 시 차수가 낮아지게 되는데 x(t)를 구하게 될 때 식이 transition from initnial state와 Effect of input으로 나뉘게 된다. 이는 state를 정의하여 미분 방정식의 초기 상태와 입력에 따른 결과를 쉽게 정리해 볼 수 있어 주어진 미분방정식의 해석을 쉽게하고 수식에 의미 부여가 가능 해진다.
* 컴퓨터로 쉽게 계산이 가능해진다.
> 다차 미분방정식을 1차 미분 방정식 여러 개로 변환이 가능해진다. 그래서 1차 미분 방정식의 연립들은 state vector를 사용하여 행렬 1차 방정식으로 변환이 가능하다. 그래서 최초의 미분방정식을 space equatino으로 변환되면 state는 의미가 부여되어 있어 수식으로부터 중간과정의 의미를 파악하며 행렬 1차 방정식으로 바뀌어 컴퓨터로 쉽게 계산이 가능해진다.
### state의 유의점  
---  
state을 정의할 때 state끼리 항등식이 되지 않도록 주의해야 한다. 아래 RLC회로에서 만약 리액터의 전류와 저항의 전류를 state로 놓는다고 가정해보자 L과 R은 서로 직렬 연결되어 있어 전류가 같아질 것이다. 그러므로 두 state 또한 항등식이 되버리고 만다. 항등식이 되게 되면 미분방정식의 연립에서 값이 계산이 되지 않아 state를 사용하여 계산이 더욱 복잡히질 가능성이 있다.   

![image](https://github.com/ji-pooh/5-/assets/144295694/9fb7d265-14dc-4e71-b90c-9b890c4847d6)

### state space equation  

---   
* 1st order state differential equation
  
![image](https://github.com/ji-pooh/Week-5-Tasks/assets/144295694/f081fc73-c64a-49a4-b1f4-f16512b1e43c)   

* n-th order state differential equation(state vector)

![image](https://github.com/ji-pooh/Week-5-Tasks/assets/144295694/5df853b8-a7bc-47dc-9aa0-d9c3fd701d55)

### summary  
---  
* state는 system 내부 상태
* state 정의 > system 수식에 의미를 부여할 수 있다.
* 다차 미분 방정식 > 1차 행렬 미분장정식
* 1차 행렬 미분 방정식은 컴퓨터가 쉽게 해결한다.
