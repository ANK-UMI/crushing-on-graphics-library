<h2>Fractal(프랙탈)</h2>
프랙탈은 일부 작은 조각이 전체와 비슷한 기하학적 형태를 띄는데, 이러한 특징을 '자기유사성'이라고 한다. 다시 말해, 자기 유사성을 갖는 기하학적 구조를 프랙탈 구조라고 한다. 브누아 망델브로가 처음 사용한 단어로, 어원은 '조각났다'라는 뜻의 라틴어 형용사 'fractus'이다. 프랙탈 구조는 가연이 가지는 기본적 구조다. 프랙탈은 수학적 도형으로 연구되기도 하는데, 이는 종종 컴퓨터 소프트웨어를 이용한 재귀적이거나 반복적인 작업에 의한 반복적인 패턴으로 만들어진다. 대표적인 프랙탈 도형으로는 망델브로 집합, 칸토어 집합, 시에르핀스키 삼각형, 페아노 곡선, 코흐 곡선 등이 있다. <br>
<br>
프랙탈의 역사는 주로 이론적 연구에서 컴퓨터 그래픽의 현대적인 적용에 이르는 길을 따른다. 

<br>
Fractal의 등장은 Algorithm만으로 Rendering할 수 있을 정도로 기술이 발전하게 된 계기가 되었다. 기존에는 Polygon으로 3d 공간을 렌더링했었다. 하지만 Polygon으로 표현하기 힘든 3D Fractal을 표현하기 위해, 모든 것을 Pixel 단위로 추적하는 Ray Marching algorithm이 고안되었다. 수학 방정식 덕분에 Code와 Data, Rendering 등 전반적으로 Optimization 될 수 있었다. 이렇듯 3D 프랙탈을 실시간으로 렌더링하는 것은 높은 기술력을 요구한다. 이전부터 게임 개발에 있어서 그래픽스 엔진의 실시간 표현과 3D 애니메이션 특수효과 기술 구현은 아주 중요한 부분이었다. 게임 개발자들 사이에서는 작은 실행 파일 크기의 게임 엔진을 만들어 시각 효과를 구현하던 '데모씬(Demoscene)'이라는 문화가 이어져오고 있다. 이들은 기술력을 과시하기 위해 데모씬에 프랙탈 모델을 사용하곤 한다. <br>
<br>
<h3>시간매개형 프랙탈(Escape-time fractals)</h3>
<h4>(1) mandelbrot set(망델브로 집합)</h4>
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

<h4>(2) julia set(줄리아 집합)</h4>
줄리아는 프랑스의 수학자로, 함수의 맵핑에 관해 20대의 나이에 논문을 쓰고 유명해졌다. 줄리아는 함수에 대해 입력 값에 대한 출력 값을 아는 것에 만족하지 않고 그 출력 값을 다시 원래의 함수에 입력시키고 또 다시 나온 출력 값을 다시 함수에 입력시키는 것을 반복하는 방식에 대해 생각했다. 그리고 그 결과가 발산하는지 혹은 어느 값에 수렴하는지에 관심을 갖게 되었다. 이는 실지로는 수학의 새로운 장르를 여는 생각이었다. 줄리아는 특히 유리 함수와의 맵핑에 관심을 두었다. <br>
줄리아의 업적은 1970년대 이후 각광받기 시작했다. 줄리아는 당시에는 컴퓨터가 없어서 집합의 경계가 어떻게 생겼는지 알 수 없었다. 1970년대 전후 IBM에 근무하는 만델브로트가 줄리아 집합을 컴퓨터로 다시 조사하던 중, 이 경계를 발견하였다. 그 이후 줄리아 집합이 유명해지게 되었다. 
그 이전까지는 수학자들은 줄리아 집합의 정의는 알았지만 아무도 집합의 경계가 그토록 복잡한 것인지에 대해서는 전혀 인식하지 못하였다. 컴퓨터의 사용이 용이한 1970년대 후반에야 인식이 된다. 줄리아 집합의 다양한 프랙탈 이미지는 수학에서 가장 근본적이고 아름다운 기하학 구조로 여겨진다. <br>
<br>
<h4>(3) 프랙탈의 정의</h4>
프랙탈 구조의 특징은 구조의 일부분을 확대해서 보아도, 확대된 부분에서 전체의 구조를 다시 찾을 수 있다는 점이다. 이러한 자기복제적인 성질을 규모불변(scale invariance) 혹은 자기유사성(self-similarity)이라고 말한다. 자기유사성을 보이는 기하학적 구조는 일찍이 칸토어(George Cantor 1845-1918)에 의해 발견되었다. 근래에 와서는 이러한 기하학적 구조를 프랙탈이라고 부르는데, 이 말은 1975년 만델브로트(Mandelbrot)의 연구저서의 제목인 라틴어 프락투스(Fractus)에서 기인한다. <br>
점(Point), 선(line), 면적(Surface), 혹은 부피(Volume)의 유클리드 기하학적 차원은 각각 0, 1, 2, 그리고 3과 같이 정수(integer)인데 반해, 자기유사성을 보이며 무리수를 포함한 '정수가 아닌 실수의 차원을 갖는 기하학적 구조'를 프랙칼이라 말한다. <br>
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
