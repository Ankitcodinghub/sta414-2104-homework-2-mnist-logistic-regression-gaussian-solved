# sta414-2104-homework-2-mnist-logistic-regression-gaussian-solved
**TO GET THIS SOLUTION VISIT:** [STA414-2104 Homework 2-Mnist logistic regression gaussian Solved](https://www.ankitcodinghub.com/product/sta414-2104-homework-2-mnist-logistic-regression-gaussian-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;96439&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;STA414-2104 Homework 2-Mnist logistic regression gaussian Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
&nbsp;

derivations, plots, and your code. You can produce the file however you like (e.g. LATEX, Microsoft Word, etc), as long as it is readable. Points will be deducted if we have a hard time reading your solutions or understanding the structure of your code. For this assignment, you should submit the filled out starter code right after your answers.

MNIST dataset. In this assignment, you will fit both generative and discriminative models using the MNIST dataset of handwritten numbers.

Each datapoint in the MNIST http://yann.lecun.com/exdb/mnist/ dataset is a 28×28 black- and-white image of a handwritten digit in {0 . . . 9}, and a label indicating which digit.

MNIST is the ’fruit fly’ of machine learning – a simple standard problem useful for comparing the properties of different algorithms. A starter Python code that loads and plots the MNIST dataset is attached. For this assignment, we will binarize the data, converting grey-scale pixels to either black or white (0 or 1) with &gt; 0.5 being the cutoff (already done in the starter code).

The starter code hw2-train.py is to be used in both questions below. You will need to write the missing parts of the functions and return it back for evaluation. Note that each missing part should be typically a few lines of code, so make sure your code is compact. When comparing models, you will need a training and test set. Build a dataset of only 2000 training samples (controlled by N_data) to use when coding or debugging, to make loading and training faster. Inspect the starter code carefully, before you start coding.

Fig 1: Samples from MNIST data set. 1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
1. Multi-class Logistic Regression Classifier – 50 pts. In this question, you will fit a discriminative model using gradient descent. Our model will be multi-class logistic regression:

exp(wkT x) p(tk = 1|x, w) = 􏰀9i=0 exp(wiT x)

Omit bias (intercept) parameters for this question.

<ol>
<li>(a) &nbsp;(5pts) How many parameters does this model have?</li>
<li>(b) &nbsp;(10pts) Write down the log-likelihood and convert it into a minimization problem over the
cross-entropy loss E. Derive the gradient of E with respect to each wk, i.e., ∇wkE(w).
</li>
<li>(c) &nbsp;(30pts) Code up a gradient descent optimizer using the starter code provided to you, and minimize the cross-entropy loss. Report the final training and the test accuracy achieved. The training must be done over the full training dataset, unless there are computational issues, in which case you can reduce the number of training samples depending on the memory available. Report the number of samples used to obtain the final result. Hint: For log_softmax function, use scipy.special.logsumexp (already imported in the starter code) or its equivalent to make your code more numerically stable. Avoid nested for loops, and instead use matrix operations to keep your code fast. Each missing chunk should be a
few lines of code!
</li>
<li>(d) &nbsp;(5pts) Plot the final weights obtained as 10 images.</li>
</ol>
What to submit?

a) Number of parameters.

b) Log-likelihood, resulting cross-entropy minimization, and the gradient.

c) Final training and test errors as well as the number of samples used in training. d) Figure containing each weight wk as an image.

e) Your entire code should be attached to the end of your answers.

2. Gaussian Discriminant Analysis – 50 pts. In this part, we train a generative model using the MNIST dataset. Assuming that the data generating distribution is Gaussian, i.e.

(2.1) p(x|Ck) = N (x | μk, Σ).

We know that the posterior p(Ck|x) can be written in terms of the softmax function

exp{ak } T

(2.2) p(Ck|x) = 􏰀j exp{aj} where ak = wk x + wk0.

Here, we also know that

(2.3) wk = Σ−1μk and wk0 = −21μTk Σ−1μk + log(p(Ck)).

(a) (5pts) Write down the log-likelihood implied by this model and find the maximum likelihood estimator (MLE) for the priors p(Ck) = πk and the class means μk, for k = 1,…,K. Note that you do not need to derive the MLE for the covariance matrix.

2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
(b) (20pts) Compute the MLEs obtained in the previous part together with the following esti- mator for the covariance matrix

(2.4) Σ􏰂=􏰁K NkΣ􏰂k where Σ􏰂k= 1 􏰁(xn−μk)(xn−μk)T, k=1 N Nk n∈Ck

where Nk is the number of images that belong to class k, and N is the total number of images. In order to make Σ􏰂 invertible, add εI for ε small e.g. ε = 1/N. Plot the means of each class as an image. Hint: In this part, if you use the entire training dataset to train your model, your computer’s memory will likely run out. Start with a small number N_data = 2000 and slowly increase it. In your final model, use as many samples as permitted by the computer memory. Report this number below. Try to avoid for loops as much as possible. Many of these operations can be written as matrix-matrix products. Take advantage of 1-of-K encoding.

(c) (15pts) Using the MLE estimators obtained in previous part as well as the posterior (2.2), make predictions on both training and test sets and report the obtained accuracy in each dataset. Also, report the number of training images used to compute the MLE estimators.

<ol start="4">
<li>(d) &nbsp;(5pts) Briefly compare the performance of this model to that of logistic regression.</li>
<li>(e) &nbsp;(5pts) Using the generative model you trained, generate 10 images from digit 0 and 10
images from digit 3.
</li>
</ol>
What to submit?

a) Log-likelihood, MLE for class means and the priors, your derivations.

b) Figure containing each class mean μk as an image.

c) Final training and test errors as well as the number of samples used in training. d) Brief comparison of final accuracies.

e) 20 images you generated.

f) Your entire code should be attached to the end of your answers.

</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</div>
