# kesci-urdu-sentiment-analysis
主要记录kesci的nlp练习赛[Roman Urdu DataSet]的两种解法。机器学习与深度学习lstm的baseline解法

competition link:https://www.kesci.com/home/competition/5c77ab9c1ce0af002b55af86/content/0

## some notes:
### 1.lstm.ipynb:   
lstm提交得分在0.83-0.84左右。lstm配套的讲解博客地址：https://blog.csdn.net/ssswill/article/details/88533623

epoch：1~5 is enough

### 2.SGD.ipynb:

SGD classifier baseline,lb=0.8651。

### 3.lgb.ipynb:
Lightgbm baseline,lb=0.8447，use bayesian optimization to find hyperparameter for lgbm。

you can improve your score base on this method.

### 4.一些心得
1.你可以尝试一些简单的模型，效果可能会更好。如朴素贝叶斯，逻辑回归等，至少目前看来是这样的。
2.可以通过一些手段使TF-idf的效果可以进一步提高，比如进一步对语句更细节的清洗，在谷歌上看过一些关于urdu清洗的论文，可以关键词搜索【roman urdu】
3.添加对表情处理我觉得会对你有帮助。
4.尝试CNN,bilstm,attention等模型。
4.虽然是练习赛，所以没有花很多的心思，但是如果钻研的话，我相信可以超过0.9。Good Luck~
