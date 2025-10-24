# iris_knn_flask

## 개요  
이 프로젝트는 파이썬의 대표적인 머신러닝 분류 예제인 scikit‑learn의 `iris` 데이터셋을 이용해 Flask 웹 애플리케이션 형태로 구현한 예제야.  
구체적으로는 KNeighborsClassifier(K-NN)을 학습하고, 웹 화면에서 입력을 받아 품종을 예측하는 흐름으로 구성돼 있어.

## 주요 기능  
- `train_model.py` : `iris` 데이터셋을 로드하고 K-NN 분류기를 학습하여 모델 파일(예: pickle)로 저장.  
- `app.py` : Flask 기반 웹 서버로, 사용자로부터 꽃의 측정값(꽃받침 길이·넓이, 꽃잎 길이·넓이)을 입력받아 학습된 모델로 품종을 예측하고 결과를 웹 화면에 출력.  
- `templates/index2.html` : 입력 폼 및 결과 표시를 담당하는 HTML 템플릿.  
- `static/images/` : 예측 결과나 설명을 위한 이미지 리소스 저장 폴더.  
- `model/` : 학습된 모델 파일 및 관련 저장 데이터를 보관하는 폴더 (예: `knn_model.pkl`)  

## 설치 및 실행 방법  
1. 저장소 복제  
   ```bash
   git clone https://github.com/kimkunwoo99/iris_knn_flask.git
   cd iris_knn_flask
