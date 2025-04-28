# math208-assignment-3-solved
**TO GET THIS SOLUTION VISIT:** [MATH208 Assignment 3 Solved](https://www.ankitcodinghub.com/product/math-208-assignment-3-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;118666&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;MATH208 Assignment 3 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
            5/5 - (2 votes)    </div>
    </div>
The assignment contains one question with 5 parts (a)-(e), each worth 10 points, for a total of 50 points. Your answers must be submitted in the form of a PDF and include both the answers to the question, along with your R code and output used to generate your answers.

Question 1 (50 points)

The basics

Logistic regression is a fundamental prediction model in statistics and modern data science. Assume that we have observed two predictors, Xi1 and Xi2 and want to predict a binary outcome Yi (i.e. Yi = 0 or Yi = 1). A logistic regression model assumes that the probability that Yi = 1 can be modelled using the following function of Xi1 = xi1 and Xi2 = xi2.

Pr(Yi = 1|Xi1 = xi1,Xi2 = xi2,θ1,θ2,θ3) = p(xi1,xi2) = .

(a) Write a function to compute p(x1,x2) for n observations which takes as arguments:

i) A vector of three parameters θ = (θ1,θ2,θ3). ii) Two predictor vectors, x1 = (x1,1,…,xn,1) and x2 = (x1,2,…xn,2)

and returns a length n vector corresponding to p(x11,p12),…p(xn1,xn2) for the corresponding θ values. Hint: You can do this without loops by subscripting for θ and using vectorized calculations for x1 and x2.

Given a dataset of n observations where we observe (Y,X1,X2) = (yi,xi1,xi2) for each observation i, one way to estimate values for θ1, θ2 and θ3 is to minimize the cross-entropy loss:

n

L(θ1,θ2,θ3) = −X[yi × log(p(xi1,xi2)) + (1 − yi) × log(1 − p(xi1,xi2))]

i=1

Note that because 0 ≤ p(x1,x2) ≤ 1, L(θ1,θ2,θ3) will be smaller when p(xi1,xi2) is close to 1 for yi = 1 and p(xi1,xi2) is close to 0 for yi = 0.

(b) Write a function to compute L(θ1,θ2,θ3) for n observations which takes as arguments:

i) A vector of three parameters θ = (θ1,θ2,θ3).

ii) Two predictor vectors, x1 = (x1,1,…,xn,1) and x2 = (x1,2,…xn,2)

iii) An outcome vector, y = (y1,…,yn)

Hint: Use your function p(x1,x2) from part (a).

CONTINUED ON NEXT PAGE

Writing a function to use with optim

optim is an opitmizer function that, by default, minimizes an argument function fn as a function of a vector first argument of fn, starting from initial values par. Other arguments for fn can be passed in …. An example function of using optim would be:

## The loss function is (x_1-a)^4 + (x_2 – b)^4, which is minimized at ## x_1 = a/2 and x_2 = b/2.

f_x &lt;- function(x,a,b){

(x[1]-a/2)^4 + (x[2]-b/2)^4 + 8

}

### optim can approximately minimize this function ### using its default optimization algorithm result&lt;-optim(par=c(10,15), fn=f_x, a=3, b=2)

## result$par: The values that minimize (x[1], x[2])

## result$value: the minimum value of f acheived at result$estimate

## result$counts: The number of iterations the algorithm took

## to converge (ignore gradient for now)

## result$code: 0 indicates a reliable convergence result, anything else

## is a problem

## result$message: A written description of any issues in converging result

$par

[1] 1.4257683 0.9559005

$value

[1] 8.000034

$counts function gradient

39 NA

$convergence [1] 0

$message

NULL

(c) Fit a logistic regression classifier to the HTRU2 data, choosing Y to be the Class values (coded as 0 and 1), X1 to be the Mean IP values and X2 to be the Mean DMSNR values using the optim() function in R. Using optim and your loss function from part (b), find the values of theta[1], theta[2], theta[3] that minimize the cross-entropy loss. Report your estimates for (θ1.θ2,θ3) and the estimated loss (and be sure to include the code that allowed you to achieve it). Note, you do not need to write a new function to do this with associated arguments, you simply can write a block of R code accomplishes the task. Starting optim at par=c(0,0,0) works well this model.

CONTINUED ON NEXT PAGE

Applying your code

(d) For this part, you should write code using a for loop (or loops) to compute the minimized cross-entropy loss for each possible pair of predictors for the HTRU2 data (note there are 82 = 28 possible models) and then store the results in a tibble with each row containing the names of the two variables used in the modelling and their cross-entropy loss). You can then arrange the rows by the value of the loss to find create a table ordered from best pairs of predictors to worst pairs according to estimated loss. Display your ordered table using the kable(.) function. Include all the code used to generate your results.

Note: starting optim at par=c(0,0,0) actually works well in all 28 models (this will not always be the case!).

Hint: I found it easiest to first use the combn() function to generate a 2 × 28 matrix where the columns contain all possible pairs pairs of names.

var_combs&lt;-combn(names(HTRU2[,-9]),2) ## -9 excludes the 9th column, the Class variable dim(var_combs)

[1] 2 28

var_combs[,1:4]

[,1] [,2] [,3] [,4]

[1,] “Mean_IP” “Mean_IP” “Mean_IP” “Mean_IP”

[2,] “SD_IP” “EK_IP” “SKW_IP” “Mean_DMSNR”
