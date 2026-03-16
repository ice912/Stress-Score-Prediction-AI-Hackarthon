9차에 대해

The notebook demonstrates a good understanding of machine learning modeling, leveraging Optuna for hyperparameter tuning and model ensembling (blending). 
However, the code suffers from fragmented data preprocessing logic, redundant operations (such as performing One-Hot Encoding twice), 
and data leakage during cross-validation because imputation is done globally before the CV splits. 
Restructuring the code using scikit-learn Pipelines will make the workflow robust, reproducible, and leak-proof.

이 노트북은 Optuna를 활용한 하이퍼파라미터 튜닝 및 모델 앙상블(블렌딩) 등 머신러닝 모델링에 대한 훌륭한 이해를 보여줍니다. 
그러나 데이터 전처리 로직이 파편화되어 있고, 중복 작업(예: 원핫 인코딩을 두 번 수행)이 있으며, 교차 검증 분할 전에 전역적으로 결측치 대체가 이루어져 
교차 검증 중 데이터 누출이 발생합니다. scikit-learn Pipelines를 사용하여 코드를 재구성하면 워크플로우가 견고하고 재현 가능하며 데이터 누출이 없는 형태로 개선될 것입니다.
