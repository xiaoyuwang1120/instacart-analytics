---
layout: page
title: Model & Performance
bigimg: /img/future.png
---

Model: XGboost & Logistic Regression

**XGboost**
```
xgb = xgboost.XGBClassifier(n_jobs=110,n_estimators=2000,max_depth=10,colsample_bytree=0.9)
xgb.fit(X_train,y_train)
```
```
XGBClassifier(base_score=0.5, booster='gbtree', colsample_bylevel=1,
       colsample_bytree=0.9, gamma=0, learning_rate=0.1, max_delta_step=0,
       max_depth=10, min_child_weight=1, missing=None, n_estimators=2000,
       n_jobs=110, nthread=None, objective='binary:logistic',
       random_state=0, reg_alpha=0, reg_lambda=1, scale_pos_weight=1,
       seed=None, silent=True, subsample=1)
```
**accuracy**
```
print("accuracy: %f" %accuracy_score(y_test[0:1000000],y_pred))

```
accuracy: 0.823846

**Logistic Regression**
```
logit=linear_model.LogisticRegression()
logit.fit(X_train,y_train)
LogisticRegression(C=1.0, class_weight=None, dual=False, fit_intercept=True,
          intercept_scaling=1, max_iter=100, multi_class='warn',
          n_jobs=None, penalty='l2', random_state=None, solver='warn',
          tol=0.0001, verbose=0, warm_start=False)
```
**accuracy**
accuracy: 0.749889


Here is the feature importance of XGBoost,
![label0](/img/11.png)
