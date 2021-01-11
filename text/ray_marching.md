<h2>Ray Marching(레이 마칭)</h2>
큰 추가비용 없이 좌우 대칭 등의 연산을 할 수 있는 등 여러가지 장점이 있다. <br>
하지만 모든 씬 혹은 씬 전체를 레이 마칭으로 처리할 수는 없다. <br>
일명 '블랙 박스'는 쉐이더 코드나 텍스처로 만들어야 한다. 즉, 직관적으로 만들지 않는다. <br>
직관적으로 만들할 수 있는 툴이 없어서 시간이 많이 걸린다. 
잘못 만드는 경우 씬이 굉장히 무거워질 수 있다. <br>
레이 마칭은 섞어서 쓸 수 있다. <br>
그러므로 모델링으로 하는 것이 더 효과적인 경우 모델링으로 제작하고, 레이 마칭으로 하는 것이 더 효과적인 경우에는 레이 마칭으로 만드는 것이 좋다. <br>
아직 레이 마칭을 직관적으로 할 수 있는 툴은 없는 듯하다. <br>
한국에서는 레이 마칭을 널리 사용하지 않는다. <br>
게임에서 구름, 안개, 그림자 등에 주로 사용되고 있다. <br>
레이 마칭은 모델링이 필요 없다(?)<br>
장난감(쉐이더 토이 등), 테크 데모?<br>
레이 마칭은 'Scene Depth'를 사용해서 폴리곤 렌더링과 쉽게 합칠 수 있다. <br>
레이 마칭은 순수한 알고리즘이며, 엔진에 종속된 기능이 아니라서 브라우저에서도 돌릴 수 있다. <br>
폴리곤으로 만들면 무거운 것도 레이마칭으로는 가볍게 돌릴 수 있다. <br>
개발 환경에 동적인 알고리즘이다. <br>
게임에서도 그리 널리 쓰이지는 않는다. <br>
특히 모바일에서는 거의 쓰지 않는다. <br>
폴리곤으로 만들 경우 굉장히 무거워질 수 있는 작업을 레이 마칭으로 해결하면 효율적이다. <br>
<br>
레이마칭으로 렌더링을 하려면, <br>
시작지점, 방향, 거리 함수가 필요하다. <br>
카메라가 시작지점, 픽셀을 방향으로 레이저를 쏘도록 만든다. <br>
씬 UV 가 있는 상태에서 <br>
UV / UV*2.0 / UV*2.0-1.0 / (uv.x, uv.y, 1.0);<br>
표면 거리 = 점과 중심 사이의 거리 - 반지름<br>
v = abs(p) - (가로/2, 세로/2, 깊이/2);<br>
거리 = max(v.x, v.y, v.z);<br>
'유니언 연산'? <br>
대칭: p.x = abs(p.x);<br>
...<br>
<br>