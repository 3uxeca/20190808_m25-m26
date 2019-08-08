# 20190808_m25-m26

m06_wine3.py
m25_DT.py
m25_RF.py
m25_GB.py
m25_XGB.py
RandomSearch, K-fold, CV 
pipeline을 제외한 세가지를 이용해서 만들기

m25_DT.py
n_jobs = 1
0.9280245022970903
{'random_state': 2, 'max_features': 5, 'max_depth': 1, 'criterion': 'gini', 'class_weight': None}
n_jobs = 2
0.9280245022970903
{'random_state': 2, 'max_features': 5, 'max_depth': 1, 'criterion': 'entropy', 'class_weight': None}
n_jobs = 3
0.9280245022970903
{'random_state': 2, 'max_features': 5, 'max_depth': 1, 'criterion': 'gini', 'class_weight': None}
n_jobs = -1
0.9280245022970903
{'random_state': 2, 'max_features': 1, 'max_depth': 1, 'criterion': 'gini', 'class_weight': None}


m25_RF.py
n_jobs = 1
0.9407861153649821
{'n_jobs': -1, 'n_estimators': 100, 'max_depth': 50, 'criterion': 'gini', 'class_weight': 'balanced_subsample'}
n_jobs = 2
0.9415518121490556
{'n_jobs': 1, 'n_estimators': 50, 'max_depth': 50, 'criterion': 'gini', 'class_weight': None}
n_jobs = 3
0.9418070444104135
{'n_jobs': -1, 'n_estimators': 50, 'max_depth': 50, 'criterion': 'gini', 'class_weight': None}
n_jobs = -1
0.9420622766717713
{'n_jobs': 2, 'n_estimators': 100, 'max_depth': 50, 'criterion': 'entropy', 'class_weight': None}


m25_GB.py
n_jobs = 1
0.925472179683512
{'random_state': 0, 'n_estimators': 10, 'max_depth': 2, 'learning_rate': 0.1}
n_jobs = 2 
0.9262378764675855
{'random_state': 3, 'n_estimators': 10, 'max_depth': 3, 'learning_rate': 0.1}
n_jobs = 3
0.9244512506380806
{'random_state': 3, 'n_estimators': 50, 'max_depth': 1, 'learning_rate': 0.1}
n_jobs = -1
0.925472179683512
{'random_state': 2, 'n_estimators': 10, 'max_depth': 2, 'learning_rate': 0.1}


m25_XGB.py
n_jobs = 1
0.9392547217968351
{'random_state': 3, 'n_jobs': -1, 'n_estimators': 100, 'max_depth': 3, 'learning_rate': 1.0, 'eval_metric': 'rmse', 'early_stopping_rounds': 10, 'base_score': 0.8}
n_jobs = 2
0.9392547217968351
{'random_state': 1, 'n_jobs': -1, 'n_estimators': 100, 'max_depth': 3, 'learning_rate': 1.0, 'eval_metric': 'rmse', 'early_stopping_rounds': 1, 'base_score': 0.8}
n_jobs = 3
0.9392547217968351
{'random_state': 3, 'n_jobs': 2, 'n_estimators': 100, 'max_depth': 3, 'learning_rate': 1.0, 'eval_metric': 'rmse', 'early_stopping_rounds': 10, 'base_score': 0.4}
n_jobs = -1
0.9392547217968351
{'random_state': 0, 'n_jobs': 1, 'n_estimators': 100, 'max_depth': 3, 'learning_rate': 1.0, 'eval_metric': 'error', 'early_stopping_rounds': 10, 'base_score': 0.6}
m08_weather1.py
m26_DT.py
m26_RF.py
m26_GB.py
m26_XGB.py


1. m26_DT.py
n_jobs = 1
R2 :  0.8829783194613108
{'splitter': 'random', 'random_state': 2, 'min_samples_split': 0.2, 'max_depth': None, 'criterion': 'friedman_mse'}
n_jobs = 2
R2 :  0.8835558607381748
{'splitter': 'best', 'random_state': 2, 'min_samples_split': 0.1, 'max_depth': 3, 'criterion': 'friedman_mse'}
n_jobs = 3
R2 :  0.8928663299930102
{'splitter': 'random', 'random_state': 1, 'min_samples_split': 0.1, 'max_depth': None, 'criterion': 'friedman_mse'}
n_jobs = -1
R2 :  0.8953754265421827
{'splitter': 'best', 'random_state': 2, 'min_samples_split': 0.1, 'max_depth': None, 'criterion': 'mse'}


2. m26_RF.py
n_jobs = 1
R2 :  0.9103527492156768
{'random_state': 2, 'n_jobs': 3, 'n_estimators': 50, 'max_features': 'sqrt', 'max_depth': 10, 'criterion': 'mae'}
n_jobs = 2
R2 :  0.9110740326913213
{'random_state': 10, 'n_jobs': 1, 'n_estimators': 100, 'max_features': 'sqrt', 'max_depth': 10, 'criterion': 'mae'}
n_jobs = 3
R2 :  0.9118156389608094
{'random_state': 2, 'n_jobs': 2, 'n_estimators': 100, 'max_features': 'sqrt', 'max_depth': 10, 'criterion': 'mae'}
n_jobs = -1
R2 :  0.9105612095094834
{'random_state': 10, 'n_jobs': 1, 'n_estimators': 50, 'max_features': 'log2', 'max_depth': 10, 'criterion': 'mae'}


3. m26_GB.py
n_jobs = 1
R2 :  0.9064264940502846
{'subsample': 1.0, 'random_state': 5, 'n_estimators': 100, 'max_features': 'sqrt', 'max_depth': 10, 'learning_rate': 0.1, 'criterion': 'mae', 'alpha': 0.5}
0.2}
n_jobs = 2
R2 :  0.9064000833785999
{'subsample': 1.0, 'random_state': 5, 'n_estimators': 100, 'max_features': 'sqrt', 'max_depth': 10, 'learning_rate': 0.2, 'criterion': 'friedman_mse', 'alpha': 0.2}
n_jobs = 3
R2 :  0.9003669079343929
{'subsample': 0.5, 'random_state': None, 'n_estimators': 50, 'max_features': 'auto', 'max_depth': 10, 'learning_rate': 0.1, 'criterion': 'mse', 'alpha': 0.5}
n_jobs = -1
R2 :  0.8976378557122408
{'subsample': 0.5, 'random_state': 5, 'n_estimators': 50, 'max_features': 'log2', 'max_depth': None, 'learning_rate': 0.1, 'criterion': 'friedman_mse', 'alpha': 




4. m26_XGB.py
n_jobs = 1
R2 :  0.9123770631330014
{'random_state': 0, 'n_jobs': -1, 'n_estimators': 50, 'max_depth': 3, 'learning_rate': 0.1, 'eval_metric': 'map', 'early_stopping_rounds': 50, 'base_score': 0.4}
n_jobs = 2
R2 :  0.911927571416754
{'random_state': 1, 'n_jobs': -1, 'n_estimators': 50, 'max_depth': 2, 'learning_rate': 0.1, 'eval_metric': 'rmse', 'early_stopping_rounds': 10, 'base_score': 0.4}
n_jobs = 3
R2 :  0.9130629274090052
{'random_state': 1, 'n_jobs': -1, 'n_estimators': 100, 'max_depth': 2, 'learning_rate': 0.1, 'eval_metric': 'error', 'early_stopping_rounds': 1, 'base_score': 0.6}
n_jobs = -1
R2 :  0.911927571416754
{'random_state': 0, 'n_jobs': 1, 'n_estimators': 50, 'max_depth': 2, 'learning_rate': 0.1, 'eval_metric': 'map', 'early_stopping_rounds': 1, 'base_score': 0.4}
