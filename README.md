# 시계열 Conditional Flow Matching 샘플링 예산

하루 합계와 급변 확률을 추정할 때, 같은 평균 네트워크 평가 횟수(NFE)에서 적분 예산을 어떻게 배분할지 살펴본 합성 실험입니다.

- 가우시안 경로에서 정확한 벡터장과 공분산을 바탕으로 Euler와 Heun의 분산·포함률 오차를 비교합니다.
- 혼합분포에서는 고정 배분과 상태를 이미 아는 오라클 배분을 비교합니다. 오라클은 계산을 배분했을 때의 가능성을 평가하는 대조군입니다.
- 실제 모델 학습과 실측 시계열 평가는 노트북의 후속 실험 계획에 적었습니다.

## 재현

Python 3.10 이상에서 아래 명령으로 JupyterLab을 실행하고 [실험 노트북](CFM_Forecast_Experiment.ipynb)의 셀을 위에서 아래로 실행합니다. 모든 입력은 노트북 안에서 생성합니다.

~~~sh
python -m pip install -r requirements.txt
jupyter lab CFM_Forecast_Experiment.ipynb
~~~
