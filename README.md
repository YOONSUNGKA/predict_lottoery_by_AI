# 회귀 모델 예측 파이프라인

이 저장소는 회귀 분석을 위한 머신러닝 파이프라인을 구현한 프로젝트입니다. 여러 머신러닝 알고리즘과 딥러닝 모델을 활용하여 주어진 입력 데이터로부터 목표 값을 정확하게 예측하는 것을 목표로 합니다.

## 주요 기능
- 데이터 로드 및 전처리
- 다양한 회귀 모델 학습 및 평가:
  - **XGBoost**
  - **LightGBM**
  - **CatBoost**
  - **랜덤 포레스트**
  - **딥러닝 모델 (TensorFlow 기반)**
- 모델 성능 비교 및 최적화
- 손실 함수 및 평가 지표:
  - **MAE (Mean Absolute Error)**
  - **F1 Score**
  - **Precision/Recall**
- 최적화 알고리즘을 통한 성능 향상 (Scipy의 `minimize` 사용)

## 설치 방법
1. 이 저장소를 클론합니다.
   ```bash
   git clone https://github.com/your-repo/predict2.git
   cd predict2
   ```
2. 필요한 패키지를 설치합니다.
   ```bash
   pip install -r requirements.txt
   ```
   > **참고:** TensorFlow, XGBoost, LightGBM, CatBoost 등이 포함되어 있습니다.

## 사용 방법
1. 데이터를 `train.csv` 및 `test.csv` 형식으로 준비합니다.
2. `predict2.ipynb` 파일을 실행하여 전체 파이프라인을 실행합니다:
   - 데이터 로드 및 전처리
   - 모델 학습 및 평가
   - 예측 결과 생성
3. 최적화된 결과를 저장하거나 추가 분석에 활용할 수 있습니다.

## 파일 구조
- `predict2.ipynb`: 전체 파이프라인 코드가 포함된 Jupyter Notebook 파일.
- `requirements.txt`: 필요한 Python 패키지 리스트.
- `data/`: 입력 데이터 (`train.csv`, `test.csv`) 디렉토리.

## 주요 기술 스택
- **프로그래밍 언어**: Python
- **라이브러리 및 프레임워크**:
  - 데이터 처리: `pandas`, `numpy`
  - 모델 학습: `XGBoost`, `LightGBM`, `CatBoost`, `scikit-learn`, `TensorFlow`
  - 최적화: `scipy`

## 평가 방법
모델 성능은 **Mean Absolute Error (MAE)** 및 **F1 Score**와 같은 지표를 사용하여 평가됩니다. 최적화된 파라미터를 적용하여 최종 결과를 도출합니다.

## 라이선스
이 프로젝트는 [MIT 라이선스](LICENSE)를 따릅니다.
