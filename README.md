<h1>KT기가지니 순간포착0.5초 게임</h1>

![genie](https://img.shields.io/badge/State-Play%20Available-blue)
현재 기가지니에서 실제 플레이하실수 있습니다

플레이영상 : https://youtu.be/3h4EERChXiI

코드 시연영상 : https://youtu.be/L2psp9c7BFs



<h2>2018 KT AI Academy<h2>

### Study AI 응용 실습 프로젝트 계획서

<a id="t.2c86e3281c3077c88e39f9044941ba9bc57b255f"></a><a id="t.0"></a>

<table class="c30">

<tbody>

<tr class="c8">

<td class="c99" colspan="1" rowspan="1">

<span class="c2">프로젝트명</span>

</td>

<td class="c60" colspan="1" rowspan="1">

<span class="c0">순간포착 0.5초</span>

</td>

</tr>

<tr class="c8">

<td class="c94" colspan="1" rowspan="1">

<span class="c2">프로젝트 요약</span>

</td>

<td class="c111" colspan="1" rowspan="1">

<span class="c0">0.5초동안 특정 사진을 사용자에게 노출하고 사진에 관한 정보로 퀴즈 문제를 제시한다. 사용자는 AI모델과 퀴즈실력을 대결한다.</span>

</td>

</tr>

<tr class="c8">

<td class="c94" colspan="1" rowspan="1">

<span class="c2">팀명</span>

</td>

<td class="c104" colspan="1" rowspan="1">

<span class="c0">KT 5G조</span>

</td>

</tr>

<tr class="c8">

<td class="c20" colspan="1" rowspan="1">

<span class="c2">팀원</span>

</td>

<td class="c115" colspan="1" rowspan="1">

<span class="c0">고은별, 신찬엽, 임정섭</span>

</td>

</tr>

</tbody>

</table>

<span class="c0"></span>

1.  <span class="c52">AI 프로젝트 개요</span>

<a id="t.35f7ce95660702f1b6e508a3620a373549aeccf5"></a><a id="t.1"></a>

<table class="c30">

<tbody>

<tr class="c8">

<td class="c44" colspan="1" rowspan="2">

<span class="c2">프로젝트 정의</span>

</td>

<td class="c64" colspan="2" rowspan="1">

<span class="c2">문제 분류</span>

</td>

<td class="c57" colspan="1" rowspan="1">

<span class="c0">Object Detection</span>

</td>

</tr>

<tr class="c14">

<td class="c22" colspan="2" rowspan="1">

<span class="c2">문제 정의</span>

</td>

<td class="c38" colspan="1" rowspan="1">

<span class="c0">주어진 사진에서 물체의 종류 및 개수에 대한 정보를 추출하여 퀴즈 문제에 맞는 답을 찾아낸다.</span>

</td>

</tr>

<tr class="c11">

<td class="c19" colspan="1" rowspan="9">

<span class="c2">모델</span>

</td>

<td class="c22" colspan="2" rowspan="1">

<span class="c2">사용 모델</span>

</td>

<td class="c10" colspan="1" rowspan="1">

<span class="c34 c105">Faster_rcnn_inception_resnet_v2_atrous</span>

</td>

</tr>

<tr class="c14">

<td class="c13" colspan="1" rowspan="7">

<span class="c2">베이스</span>

<span class="c2">모델</span>

<span class="c2"></span>

</td>

<td class="c17" colspan="1" rowspan="1">

<span class="c2">논문정보</span>

<span class="c2">(Citation)</span>

</td>

<td class="c38" colspan="1" rowspan="1">

<span class="c0">Faster R-CNN: Towards Real-Time Object Detection with Region Proposal Networks</span>

<span class="c0"></span>

</td>

</tr>

<tr class="c14">

<td class="c17" colspan="1" rowspan="1">

<span class="c2">데이터</span>

</td>

<td class="c10" colspan="1" rowspan="1">

<span class="c0">PASCAL VOC 2007, 2012, and MS COCO datasets</span>

</td>

</tr>

<tr class="c14">

<td class="c17" colspan="1" rowspan="1">

<span class="c2">입력</span>

</td>

<td class="c38" colspan="1" rowspan="1">

<span class="c0">(크기 상관 없음) 2D image</span>

</td>

</tr>

<tr class="c14">

<td class="c17" colspan="1" rowspan="1">

<span class="c2">출력</span>

</td>

<td class="c10" colspan="1" rowspan="1">

<span class="c0">감지한 object label, object의 좌표값</span>

</td>

</tr>

<tr class="c14">

<td class="c17" colspan="1" rowspan="1">

<span class="c2">아키텍쳐</span>

</td>

<td class="c38" colspan="1" rowspan="1">

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 340.00px; height: 216.00px;">![](images/image3.png)</span>

<span class="c0"></span>

<span class="c0"></span>

</td>

</tr>

<tr class="c14">

<td class="c17" colspan="1" rowspan="1">

<span class="c2">성능지표</span>

</td>

<td class="c10" colspan="1" rowspan="1">

<span class="c0">Speed(ms) / mAP</span>

</td>

</tr>

<tr class="c14">

<td class="c17" colspan="1" rowspan="1">

<span class="c2">성능</span>

</td>

<td class="c38" colspan="1" rowspan="1">

<span class="c0">620 / 37</span>

</td>

</tr>

<tr class="c48">

<td class="c22" colspan="2" rowspan="1">

<span class="c2">코드 주소</span>

</td>

<td class="c10" colspan="1" rowspan="1">

<span class="c0">https://github.com/tensorflow/models/blob/master/research/object_detection/</span>

</td>

</tr>

<tr class="c8">

<td class="c19" colspan="1" rowspan="3">

<span class="c2">데이터</span>

</td>

<td class="c22" colspan="2" rowspan="1">

<span class="c2">사용 데이터</span>

</td>

<td class="c38" colspan="1" rowspan="1">

<span class="c0">상업적 사용이 가능한 사진데이터(CC0 license)</span>

</td>

</tr>

<tr class="c8">

<td class="c22" colspan="2" rowspan="1">

<span class="c2">데이터 수</span>

</td>

<td class="c10" colspan="1" rowspan="1">

<span class="c0">100장~200장(미정)</span>

</td>

</tr>

<tr class="c48">

<td class="c22" colspan="2" rowspan="1">

<span class="c2">데이터 주소</span>

</td>

<td class="c38" colspan="1" rowspan="1">

<span class="c45 c95">[https://drive.google.com/drive/folders/1FtnNXEsbt_DffMjZemzYLRzELifnHKpL](https://www.google.com/url?q=https://drive.google.com/drive/folders/1FtnNXEsbt_DffMjZemzYLRzELifnHKpL&sa=D&ust=1570631463616000)</span>

<span class="c0"></span>

</td>

</tr>

<tr class="c8">

<td class="c19" colspan="1" rowspan="4">

<span class="c2">AI</span>

<span class="c2">개발 스펙</span>

</td>

<td class="c22" colspan="2" rowspan="1">

<span class="c2">프레임워크(버전)</span>

</td>

<td class="c10" colspan="1" rowspan="1">

<span class="c0">Flask, Tensorflow 1.7, 기가지니 SDK</span>

</td>

</tr>

<tr class="c48">

<td class="c22" colspan="2" rowspan="1">

<span class="c2">언어(버전)</span>

</td>

<td class="c38" colspan="1" rowspan="1">

<span class="c0">Python 3, Javascript</span>

</td>

</tr>

<tr class="c48">

<td class="c22" colspan="2" rowspan="1">

<span class="c2">개발환경(IDE)</span>

</td>

<td class="c10" colspan="1" rowspan="1">

<span class="c0">Spyder, SublimeText , Jupyter notebook</span>

</td>

</tr>

<tr class="c37">

<td class="c22" colspan="2" rowspan="1">

<span class="c2">기타 스펙 (docker, Cuda,cuDnn, openCV 등)  </span>

</td>

<td class="c38" colspan="1" rowspan="1">

<span class="c0">Cuda 8.0</span>

</td>

</tr>

<tr class="c37">

<td class="c19" colspan="1" rowspan="4">

<span class="c2">데모 스펙</span>

<span class="c63">*구현 관련 항목 모두 작성</span>

<span class="c2"></span>

<span class="c2"></span>

<span class="c2"></span>

</td>

<td class="c80" colspan="2" rowspan="1">

<span class="c2">서버</span>

</td>

<td class="c10" colspan="1" rowspan="1">

<span class="c0">apache2( 추후 ucloud로 변경 가능성 높음)</span>

</td>

</tr>

<tr class="c37">

<td class="c22" colspan="2" rowspan="1">

<span class="c2">웹/모바일 등</span>

</td>

<td class="c38" colspan="1" rowspan="1">

<span class="c0">웹</span>

</td>

</tr>

<tr class="c37">

<td class="c80" colspan="2" rowspan="1">

<span class="c2">DB</span>

</td>

<td class="c10" colspan="1" rowspan="1">

<span class="c0">Mysql</span>

</td>

</tr>

<tr class="c37">

<td class="c90" colspan="2" rowspan="1">

<span class="c2">하드웨어</span>

</td>

<td class="c106" colspan="1" rowspan="1">

<span class="c0">기가지니 ver1</span>

</td>

</tr>

</tbody>

</table>

<span class="c46"></span>

1.  <span class="c52">AI 프로젝트 상세 내용</span>

<a id="t.64faf57547b23ef65f47a2831d2ab30cc2a5b22f"></a><a id="t.2"></a>

<table class="c30">

<tbody>

<tr class="c8">

<td class="c44" colspan="1" rowspan="2">

<span class="c2">배경</span>

</td>

<td class="c64" colspan="2" rowspan="1">

<span class="c2">필요성</span>

</td>

<td class="c83" colspan="1" rowspan="1">

<span class="c0">기가지니 내 게임컨텐츠가 질적, 양적으로 부족하다</span>

</td>

</tr>

<tr class="c48">

<td class="c22" colspan="2" rowspan="1">

<span class="c45 c56">KT/그룹사</span> <span class="c2">연관성</span>

</td>

<td class="c53" colspan="1" rowspan="1">

<span class="c0">전사적 차원에서 역량을 집중하는 기가지니의 컨텐츠를 개발함으로서 기가지니에 대한 관심을 높일 수 있을 것이다.</span>

</td>

</tr>

<tr class="c8">

<td class="c19" colspan="1" rowspan="1">

<span class="c2">목표</span>

</td>

<td class="c79" colspan="3" rowspan="1">

<span class="c0">기본적으로 흥미를 유발하는 게임 개발을 목표로 한다. 또한, AI 프레임워크는 tensorflow 기반이고 기가지니는 javascript 기반인데, 환경이 다른 기능들을 적절히 함께 사용할 수 있도록 한다.</span>

</td>

</tr>

<tr class="c8">

<td class="c19" colspan="1" rowspan="1">

<span class="c2">상세설명</span>

</td>

<td class="c40" colspan="3" rowspan="1">

<span class="c0">기가지니에 들어갈 게임을 기획하고 개발한다. 기가지니 특성상 음성으로 제어할 수 있는 게임이어야 하기 떄문에 퀴즈 형식의 게임을 기획하였다.</span>

<span class="c0">0.5초간 노출되는 사진에 관한 퀴즈가 출제되면 사용자와 AI 가 퀴즈점수를 겨루게 되는 게임을 기획하였다. 사람 및 물체가 담긴 이미지를 사용자에게 0.5초 간 보여준다. 0.5초 후 이미지가 사라지면 관련된 퀴즈 문제와 보기 3개가 제시된다. 문제 유형은 '종류 맞추기', '개수 맞추기', '없는 것 고르기', '가장 많은 것 고르기' 및 '여러 이미지 보고 없는 것 고르기'로 이루어져 있다. 추후 더 많은 문제 유형을 추가해 사용자의 흥미를 유발할 예정이다. 난이도는 초급, 중급, 고급으로 사진에 있는 물체 개수, 종류의 수, 문제 유형 등에 따라 나뉜다.</span>

<span class="c0">사용자가 문제를 읽고 응답하는 동안 AI 모델은 object detection을 통해 물체 종류와 개수를 파악하여 해당하는 보기를 고른다. 만약 AI 모델이 예측한 답과 일치하는 보기가 없다면 랜덤으로 보기를 선택하도록 한다. AI 모델이 시간 내에 예측을 끝내지 못할 경우 대답하지 않은 것으로 처리한다. 사용자와 AI 모델 둘 중 한 쪽만 정답을 맞춰도 다음 문제로 넘어간다. 둘 다 정답을 맞추지 못할 시, 이미지를 0.5초 간 한 번 더 보여주는 힌트를 제공한다. 이 때, AI는 이전에 선택했던 보기와 다른 보기를 랜덤으로 선택하거나 첫 번째 시도에서 다 하지 못했던 예측을 마저 완료하도록 한다. 두 번째 시도 후에는 사용자/AI의 정답 유무와 관계 없이 다음 문제로 넘어간다.</span>

<span class="c0">게임 한 세트는 5문제로 구성되어있고, 한 세트에는 겹치는 이미지가 없도록 구성한다. 첫 번째 시도에서 문제를 맞추면 20점, 두 번째 시도에서는 10점, 문제를 맞추지 못하면 0점을 누적점수에 더한다. 5문제를 다 푼 이후에는 누적 점수를 계산하여 사용자와 AI 중 승자를 가린다.</span>

<span class="c0">본 프로젝트에는 AI 모델의 성능, 속도 개선 및 기가지니 SDK와 AI 모델 결합이라는 기술적 과제가 있다. 현재 모델이 한 장의 사진을 detect하는 데 있어서 약 7~11초라는 시간이 소요되는데, 사용자가 이미지를 보고 응답을 마치기까지 약 9초 정도의 시간이 걸린다는 점을 감안한다면 속도 개선이 본 게임 실현에 있어서 주요 과제라고 볼 수 있다. 또한, 서로 다른 환경의 기가지니 SDK와 AI 모델을 결합시키는 것 역시 구현에 있어서 필수적인 과제다.</span>

<span class="c0"></span>

<span class="c0">본 프로젝트는 실제 게임상용화를 최종 목표로 하고 있으며, 기획 및 개발을 넘어 디자인 측면까지 UI/UX KT전문가와 협업해 하나의 완성도 있는 웹앱을 출시할 계획이다.</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 475.00px; height: 170.67px;">![](images/image5.jpg)</span>

<span class="c0"></span>

</td>

</tr>

<tr class="c8">

<td class="c19" colspan="1" rowspan="5">

<span class="c2">설계모델</span>

<span class="c63">*여러 개일 경우 모두 명시</span>

<span class="c2"></span>

</td>

<td class="c13" colspan="1" rowspan="5">

<span class="c2">모델 : faster-rcnn</span>

</td>

<td class="c17" colspan="1" rowspan="1">

<span class="c2">역할</span>

</td>

<td class="c28" colspan="1" rowspan="1">

<span class="c0">사용자의 상대역할로 사진이 input으로 주어지면 물체의 label과 개수를 구한다.</span>

</td>

</tr>

<tr class="c8">

<td class="c17" colspan="1" rowspan="1">

<span class="c2">구조</span>

</td>

<td class="c53" colspan="1" rowspan="1">

<span class="c0">1.의 아키텍쳐 참고</span>

</td>

</tr>

<tr class="c8">

<td class="c17" colspan="1" rowspan="1">

<span class="c2">입력</span>

</td>

<td class="c28" colspan="1" rowspan="1">

<span class="c0">2D 이미지</span>

</td>

</tr>

<tr class="c8">

<td class="c17" colspan="1" rowspan="1">

<span class="c2">출력</span>

</td>

<td class="c53" colspan="1" rowspan="1">

<span class="c0">감지한 object label, object의 개수</span>

</td>

</tr>

<tr class="c8">

<td class="c17" colspan="1" rowspan="1">

<span class="c2">평가지표</span>

</td>

<td class="c28" colspan="1" rowspan="1">

<span class="c0">없음</span>

</td>

</tr>

<tr class="c8">

<td class="c19" colspan="1" rowspan="2">

<span class="c2">기대효과</span>

</td>

<td class="c22" colspan="2" rowspan="1">

<span class="c2">기술적 측면</span>

</td>

<td class="c53" colspan="1" rowspan="1">

<span class="c0">기가지니 SDK와 AI모델의 결합</span>

</td>

</tr>

<tr class="c8">

<td class="c22" colspan="2" rowspan="1">

<span class="c2">사업적 측면</span>

</td>

<td class="c28" colspan="1" rowspan="1">

<span class="c0">기가지니에 대한 관심 증대 -> KT의 기가지니 보급 목표 달성 기여</span>

</td>

</tr>

<tr class="c8">

<td class="c19" colspan="1" rowspan="2">

<span class="c2">문제해결</span>

</td>

<td class="c22" colspan="2" rowspan="1">

<span class="c2">예상 어려움</span>

</td>

<td class="c53" colspan="1" rowspan="1">

<span class="c0">프레임워크가 다른 프로그램들의 혼합</span>

</td>

</tr>

<tr class="c8">

<td class="c90" colspan="2" rowspan="1">

<span class="c2">해결 방안</span>

</td>

<td class="c81" colspan="1" rowspan="1">

<span class="c0">WSGI 사용</span>

</td>

</tr>

</tbody>

</table>

<span class="c46"></span>

1.  <span class="c52">AI 프로젝트 일정</span>

<a id="t.a80eb39dd1eae8346c0705f9ca945afa23fd4905"></a><a id="t.3"></a>

<table class="c30">

<tbody>

<tr class="c100">

<td class="c91" colspan="1" rowspan="1">

<span class="c2">세부과제</span>

</td>

<td class="c85" colspan="7" rowspan="1">

<span class="c2">1주차/2주차</span>

</td>

<td class="c70" colspan="7" rowspan="1">

<span class="c2">3주차/4주차</span>

</td>

<td class="c97" colspan="7" rowspan="1">

<span class="c2">5주차/6주차</span>

</td>

<td class="c55" colspan="2" rowspan="1">

<span class="c2">비고</span>

</td>

</tr>

<tr class="c47">

<td class="c25" colspan="1" rowspan="1">

<span class="c2">1.서비스 기획 및 구체화</span>

</td>

<td class="c26" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c26" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c26" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c26" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c98" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c75" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c75" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c75" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c9" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c23" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

</tr>

<tr class="c37">

<td class="c25" colspan="1" rowspan="1">

<span class="c2">2.기존 기가지니 앱 분석</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c4" colspan="1" rowspan="1">

<span class="c0 c24"></span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0 c24"></span>

</td>

<td class="c98" colspan="1" rowspan="1">

<span class="c0 c24"></span>

</td>

<td class="c98" colspan="1" rowspan="1">

<span class="c0 c24"></span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0 c24"></span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c4" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c35" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c35" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c4" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c4" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c4" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c4" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c4" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c18" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c76" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

</tr>

<tr class="c37">

<td class="c25" colspan="1" rowspan="1">

<span class="c2">3.기존 기가지니 앱 응용해 서비스 프로토타입 개발</span>

</td>

<td class="c42" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c42" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c42" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c42" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c75" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c98" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c75" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c75" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c29" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c9" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c23" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

</tr>

<tr class="c37">

<td class="c25" colspan="1" rowspan="1">

<span class="c2">4.AI모델과 프로토타입 모델 결합</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c4" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c4" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c35" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c35" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c4" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c98" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c35" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c4" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c4" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c4" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c4" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c4" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c18" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c76" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

</tr>

<tr class="c37">

<td class="c112" colspan="1" rowspan="1">

<span class="c2">5\. 서비스 고도화(UX 및 디자인 개선)</span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c69" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c69" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c62" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c62" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c69" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c69" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c69" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c69" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c67" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c61" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c61" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c67" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c67" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c67" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c67" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c67" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c93" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c114" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

</tr>

</tbody>

</table>

<span class="c46"></span>

1.  <span class="c52">팀원 및 역할분담</span>

<a id="t.1f74c962ed439e5c811d65ef53078f32030a82f2"></a><a id="t.4"></a>

<table class="c30">

<tbody>

<tr class="c14">

<td class="c74" colspan="1" rowspan="1">

<span class="c2">구분</span>

</td>

<td class="c72" colspan="1" rowspan="1">

<span class="c2">이름</span>

</td>

<td class="c65" colspan="1" rowspan="1">

<span class="c2">담당분야</span>

</td>

<td class="c86" colspan="1" rowspan="1">

<span class="c2">전문성</span>

</td>

</tr>

<tr class="c14">

<td class="c49" colspan="1" rowspan="1">

<span class="c2">팀장</span>

</td>

<td class="c17" colspan="1" rowspan="1">

<span class="c0">고은별</span>

</td>

<td class="c110" colspan="1" rowspan="1">

<span class="c0">AI모델, 디자인, 기획</span>

</td>

<td class="c103" colspan="1" rowspan="1">

<span class="c0">통계 기반 AI 모델링</span>

</td>

</tr>

<tr class="c37">

<td class="c49" colspan="1" rowspan="1">

<span class="c2">팀원</span>

</td>

<td class="c17" colspan="1" rowspan="1">

<span class="c0">신찬엽</span>

</td>

<td class="c16" colspan="1" rowspan="1">

<span class="c0">기가지니SDK 웹앱, 디자인, 기획</span>

</td>

<td class="c50" colspan="1" rowspan="1">

<span class="c0">SW개발</span>

</td>

</tr>

<tr class="c14">

<td class="c78" colspan="1" rowspan="1">

<span class="c2">팀원</span>

</td>

<td class="c31" colspan="1" rowspan="1">

<span class="c0">임정섭</span>

</td>

<td class="c54" colspan="1" rowspan="1">

<span class="c0">AI모델, 기가지니 SDK웹앱</span>

</td>

<td class="c71" colspan="1" rowspan="1">

<span class="c0">오픈소스 이해 및 응용</span>

</td>

</tr>

</tbody>

</table>

<span class="c46"></span>

1.  <span class="c52">데모 시나리오 및 UI</span>

<a id="t.709eb2545ce10a16644785aced767487f3ccce31"></a><a id="t.5"></a>

<table class="c30">

<tbody>

<tr class="c8">

<td class="c107" colspan="2" rowspan="1">

<span class="c45">데모 시나리오 및 데모 UI</span>

</td>

</tr>

<tr class="c8">

<td class="c51" colspan="2" rowspan="1">

<span class="c0">(이미지 첨부)</span>

<span class="c66">*UI툴 참고</span>

<span class="c95 c117">[https://ovenapp.io/view/IXBYM2skGAw0bTneiQgcjNi5XkMie5ps/](https://www.google.com/url?q=https://ovenapp.io/view/IXBYM2skGAw0bTneiQgcjNi5XkMie5ps/&sa=D&ust=1570631463737000)</span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

1.  <span class="c34">게임 시작 후 [초급,중급,고급] 중 난이도를 선택한다.</span>

<span class="c0"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 547.00px; height: 288.00px;">![](images/image4.png)</span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

1.  <span class="c0">난이도 선택 후 문제를 내기 위한 사진이 0.5초간 보여진다.</span>

<span class="c0"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 547.00px; height: 273.33px;">![](images/image7.jpg)</span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

1.  <span class="c0">사진이 사라지고 문제와 보기 3개가 나타난다.</span>

<span class="c0"></span>

<span class="c0"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 547.00px; height: 269.33px;">![](images/image6.png)</span>

<span class="c46"></span>

<span class="c46"></span>

<span class="c46"></span>

<span class="c46"></span>

<span class="c46"></span>

1.  <span class="c0">문제에 대한 답을 말하고, 사진과 함께 답을 확인한다.</span>

<span class="c46"></span>

<span class="c46"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 547.00px; height: 317.33px;">![](images/image2.png)</span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>

1.  <span class="c0">2-4 과정을 5문제동안 반복 후 AI와 최종 점수를 비교하여 승패를 가린다.</span>

<span class="c0"></span>

<span class="c0">        </span>

1.  <span class="c0">승패를 가린 후, [다시하기] 또는 [나가기]를 선택한다.</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 547.00px; height: 294.67px;">![](images/image1.png)</span>

</td>

</tr>

</tbody>

</table>

<span class="c46"></span>