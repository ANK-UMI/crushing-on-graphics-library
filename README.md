<h2>Fractal(프랙탈)</h2>
프랙탈은 일부 작은 조각이 전체와 비슷한 기하학적 형태를 띄는데, 이러한 특징을 '자기유사성'이라고 한다. 다시 말해, 자기 유사성을 갖는 기하학적 구조를 프랙탈 구조라고 한다. 브누아 망델브로가 처음 사용한 단어로, 어원은 '조각났다'라는 뜻의 라틴어 형용사 'fractus'이다. 프랙탈 구조는 가연이 가지는 기본적 구조다. 프랙탈은 수학적 도형으로 연구되기도 하는데, 이는 종종 컴퓨터 소프트웨어를 이용한 재귀적이거나 반복적인 작업에 의한 반복적인 패턴으로 만들어진다. 대표적인 프랙탈 도형으로는 망델브로 집합, 칸토어 집합, 시에르핀스키 삼각형, 페아노 곡선, 코흐 곡선 등이 있다. <br>
<br>
프랙탈의 역사는 주로 이론적 연구에서 컴퓨터 그래픽의 현대적인 적용에 이르는 길을 따른다. 

<br>
Fractal의 등장은 Algorithm만으로 Rendering할 수 있을 정도로 기술이 발전하게 된 계기가 되었다. 기존에는 Polygon으로 3d 공간을 렌더링했었다. 하지만 Polygon으로 표현하기 힘든 3D Fractal을 표현하기 위해, 모든 것을 Pixel 단위로 추적하는 Ray Marching algorithm이 고안되었다. 수학 방정식 덕분에 Code와 Data, Rendering 등 전반적으로 Optimization 될 수 있었다. 이렇듯 3D 프랙탈을 실시간으로 렌더링하는 것은 높은 기술력을 요구한다. 이전부터 게임 개발에 있어서 그래픽스 엔진의 실시간 표현과 3D 애니메이션 특수효과 기술 구현은 아주 중요한 부분이었다. 게임 개발자들 사이에서는 작은 실행 파일 크기의 게임 엔진을 만들어 시각 효과를 구현하던 '데모씬(Demoscene)'이라는 문화가 이어져오고 있다. 이들은 기술력을 과시하기 위해 데모씬에 프랙탈 모델을 사용하곤 한다. <br>
<br>
<h3>시간매개형 프랙탈(Escape-time fractals): mandelbrot set(망델브로 집합), julia set(줄리아 집합)</h3>
<h4>mandelbrot set</h4>
The Mandelbulb is a three-dimensional fractal, constructed by Daniel White and Paul Nylander using spherical coordinates in 2009. A canonical 3-dimensional Mandelbrot set does not exist, since there is no 3-dimensional analogue of the 2-dimensional space of complex numbers. It is possible to construct Mandelbrot sets in 4 dimensions using quaternions and bicomplex numbers. <br>
<br>
<ul>
<li>Quadratic formula</li>
<li>Cubic formula</li>
<li>Quintic formula</li>
<li>Power nine formula</li>
<li>Spherical formula</li>
</ul>
<br>
See also Mandelbulb, Mandelbox, fractals by Hausdorff dimension. <br>
<br>
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/KochFlake.svg/280px-KochFlake.svg.png">
<br>
Benoit S. Mandelbrot(1924 ~2010)의 2D 프랙탈 만델브로트 집합처럼 흥미롭고 무한히 복잡한 경계를 가진 3D 프랙탈을 찾으려는 시도가 있었지만 그 결과는 신통치 않았다. 하지만 2009년 Fractalforum.com 의 3D Fractal 쓰레드를 통해서 Daniel White와 Paul Nylander가 마침내 'Mandelbulb'를 발견했다. <br>
<br>

<h3>반복함수계(Iterated function system)</h3>
<ul>
<li>칸토어 집합</li>
<li>시에르핀스키 삼각형</li>
<li>시에르핀스키 카펫</li>
<li>코흐 곡선</li>
<li>페아노 곡선</li>
</ul>

<br>


<br>
<h3>Menger sponge(멩거 스펀지)</h3>


<br>
<br>
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
<h2>Power of two(2ⁿ, 2의 거듭제곱)</h2>
<img src = "https://upload.wikimedia.org/wikipedia/commons/thumb/1/16/Powers_of_two_cuboids.svg/440px-Powers_of_two_cuboids.svg.png"><br>
<br>
In mathematics, a power of two is a number of the form  2ⁿ(2의 n승) where 'n' is an integer, 
that is, the result of exponentiation with number two as the base and integer 'n' as the exponent(거듭 제곱). <br>
<br>
In a context where only integers are considered, 'n' is restricted to non-negative values, so we have 1, 2, and 2 multiplied by itself a certain number of times. <br>
<br>
Because 'two' is the base of the binary numeral system, 'powers of two' are common in computer science. <br>
Written in binary, a power of two always has the form 100…000 or 0.00…001, just like a power of ten in the decimal system. <br>
<br>
Two to the power of n, written as 2n, is the number of ways the bits in a binary word of length n can be arranged. <br>
A word, interpreted as an unsigned integer, can represent values from 0 (000…0002) to 2n − 1 (111…1112) inclusively. <br>
Corresponding signed integer values can be positive, negative and zero; see signed number representations. <br>
Either way, one less than a power of two is often the upper bound of an integer in binary computers. <br>
As a consequence, numbers of this form show up frequently in computer software. <br>
<br>
As an example, a video game running on an 8-bit system might limit the score or the number of items the player can hold to 255—the result of using a byte, which is 8 bits long, to store the number, giving a maximum value of 28 − 1 = 255 <br>
<br>

* 2의 0승 = 1
* 2의 1승 = 2
* 2의 2승 = 4
* 2의 3승 = 8
* 2의 4승 = 16
* 2의 5승 = 32
* 2의 6승 = 64
* 2의 7승 = 128
* 2의 8승 = 256
* 2의 9승 = 512
* 2의 10승 = 1,024
* 2의 11승 = 2,048
* 2의 12승 = 4,096
* 2의 13승 = 8,192
* 2의 14승 = 16,384
* 2의 15승 = 32,768

<br>
