# Tree_Based_Methods

*__Tree based method__* is one of the most popular tools to use in the field of data science. It can be used for both *regression* as well as for *classification* tasks. It is the algorithmic backbone for libraries such as XGBoost, which continue to outperform other DL methods on various Kaggle competitions.

### Let's see how it works.

#### Tree methods works by straifying or segmenting the predictor space into a number of smaller regions or smaller subspace

With any given dataset, we have X1, X2, ....., Xp. The set of predictors, which generate a predictor space with p predictors/features. This can be represented by a rank p tensor. 

*an example for this would be maping displacement with respect to time on a cartesian coordinate system, where as time progresses, we can traverse within the x, y, and z axises defined space, each of which tells us the unique information of our location along the specific axis or predictor.*

__Step 1:__ We divide the predictor space into J distinct and non-overlapping regions, R1, R2,...., RJ

__Step 2:__ For every oberservation that falls into the region Rj, we make the same prediction, which is taken to be simple the mean of the response value for the training observation in Rj. The shape of the segmented region doesn't matter. But intuitively, hyper-rectangle is easiest to work with mathimatically.

### Idea: Segment the regions R1, ...., RJ that minimizes the residual sum of squares.


![Image of Tree_Formulae](https://github.com/bosgithub/Tree_Based_Methods/Tree_Formulae.png)
