# carbon
팀 프로젝트 - 탄소계산기 시각화 및 보고서 웹페이지 제작 및 간단한 앱

프로젝트 기간 :2023-11-07 ~ 2023-012-~

프로젝트 도구 :Spring-tool-suite, SQLDeveloper, PyCharm, MySQL, VsCode, Jenkins 

사용 기술 :Spring, MVC모델, JQuery, Bootstrap, 머신러닝

사용 언어 :JAVA, JSP, HTML/CSS/JS, SQL, Python
사용한 데이터:대한민국가구평균전력(한전API를통해 가져옴)
            : 다른가구 평균에너지사용량(탄소발자국 참조)

[맡은부분 설명] 
               자신의 사는 지역의 평균가구의 평균전력사용량을 볼수있으며 예측된 모델을 통해 2023년 12월까지의 예측사용량을 볼수있다.
               계산기부분에서 사용자는 가스 전기 수도 사용량을 입력하고 자신의 정보를 입력하면 평균적인 다른 사용자들과의 사용량을
               비교하교 사용자의 부분별 탄소배출량과 탄소배출량을 나무로 환산했을시의 결과를 차트를 통해 시각화해서 보여주고
               PDF 형식으로 최종적으로 보고서 형식으로 볼수 있다.


[구현한 부분 화면 ]

![model](https://github.com/tjddndchl/carbon/assets/104568586/0b55c878-2244-4088-893c-0ba0a6ea1d82)
      VO를 통해 database와 연동하여 년도 지역 시군구 를 선택시 선택한 값에 따른
      가구 평균전력사용량과 머신러닝 모델을 통해 만든 예측 사용량을 서로 비교하여 그래프로 보여준다.

      


![image](https://github.com/tjddndchl/carbon/assets/104568586/fa2b7208-a4e5-466a-a084-c979779b6ade)
사용자가 자신의 사용량을 입력하고 계산을 누르면 환산하여 보여준다.
계산한 결과는 로컬스토리지를 통해 저장한다.





![information](https://github.com/tjddndchl/carbon/assets/104568586/10595953-56fe-468b-8f05-bb6442fec0ff)
사용자의 정보를 입력시 다른가구의 평균 사용량을 데이터를 가져온다.



![result1](https://github.com/tjddndchl/carbon/assets/104568586/abdc122b-3b6d-44a2-bac7-49c9c83e3f60)

사용량 분석화면




![result2](https://github.com/tjddndchl/carbon/assets/104568586/f36d0ade-b959-4b05-ab15-1b6896276cda)
실천 목표화면 솔루션 선택시 솔루션의 사용량과 감소하는 요금량
그리고 솔루션 적용해서 감소한 목표량으로 그래프로 시각화해준다.



![result3](https://github.com/tjddndchl/carbon/assets/104568586/976ec5ac-7e1b-4413-b82e-9cd49a2e1b89)

종합평가 화면

보고서이동시 보고서 페이지로 이동하고

![report3](https://github.com/tjddndchl/carbon/assets/104568586/3134f0af-9a5c-400a-8e24-5200b3ce8618)

보고서 다운시 만들어 놓은 양식으로 보고서를 pdf파일로 내려받을수있다.

