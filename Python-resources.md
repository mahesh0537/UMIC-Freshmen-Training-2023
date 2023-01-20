<p>
<img align="left" src="assets/UMIC.png" alt="UMIC logo" style="height: 100px; width:400px;">
<img align="right" src="assets/IITB-logo.png"alt="UMIC logo" style="height: 100px; width:100px;"/>
</p>

<br>
<br>
<br>
<br>
<br>
<br>

# **Training: Python**

**Python is the core language of ROS (Robot Operating System). Robot's motion planning,
manipulation, navigation, localization, image processing, physics simulation, etc are research
programmed commonly using Python.**
<br>
<span style="color:red">
*We encourage you to refer material apart from the stuff given below as well to expand
your understanding. We have tried to curate a list of resources we found would utilize
your time the best way.
Please read the entire document before beginning with anything.*
</span>

## **Introduction:**
* we recommend you to go through this [course](https://www.coursera.org/specializations/python-3-programming#courses) in Coursera if you are completely new or not at all
confident with programming especially with C++. \
*Watch only the videos, Don’t get deviated with the Reading and Project parts in the course*
  * In the 1st course:
    * Do only week 1 and week 2 and basic if-else loops in week 3
  * In the 2nd course:
    * Do only Dictionary basics in week 2
    * Do week 3 and week 4 only
  * In the 4th Course:
    * Do week 1 and week 2 only
**You should skip course no.3 in this specialization i.e Data Collection and Preprocessing
and course no. 5.** 

**NOTE:** For accessing a single course from a specialization course,you can select a single course
and click on enrol and then click on “audit the single course”. 

You can follow this [youtube tutorial](https://www.youtube.com/watch?v=_uQrJ0TkZlc) if you are
already familiar with little Python or confident in basic programming, follow this video at your comfortable speed (>1x) asap and complete it in a day. He uses Python 3xx version. Make sure you are well versed with classes if you are following this. 

Also after you complete this go through this [short lecture](https://www.youtube.com/watch?v=ZDa-Z5JzLYM&list=PL-osiE80TeTsqhIuOqKhwlXsIBIdSeYtc) series for reference for **OOP concepts** assuming you haven't understood it properly (no need if you have done the coursera course), **This is very important make sure you pay good attention as you will come across this very much
frequently.**

## Installation:

For windows: You can install python as shown in the video above (recommended) or can do it from [here](https://www.python.org/downloads/windows/)
Note: In ubuntu you already have a python version so you could just go into terminal and type python and enter. But you will be needing an editor for sure. (You may have 2 different versions of python in ubuntu, if you are getting python 2.7 with python, try python3 you will see python 3.x, we use python3.x only)

### Visual Studio Code : Text Editor
We recommend you use Visual Studio Code as your Primary code editor instead of PyCharm as
shown in the videos. You can watch short [videos](https://www.youtube.com/watch?v=h0HbFnb8bC8&ab_channel=CodingGeek) to run python in
vscode. Also Visual Studio Code is very flexible when it comes to dealing with GitHub
Repositories. (*Never heard of git? No worries, we’ll catch on it once you finish python*)

#### Practice is all you need now

## Important Libraries in Python
**We use PIP to manage libraries, follow [this](https://www.w3schools.com/python/python_pip.asp) short tutorial to get handy with PIP**

1. Numpy: [Tutorial Video](https://youtu.be/GB9ByFAIAH4)

   for loop in python is slow af, so we need some way to vectorize our process of heavy number crunching workload.

2. Pandas: [Tutorial Video](https://youtu.be/vmEHCJofslg)

    See the “Working with CSV and Excel files” part only

3. OS: [Tutorial Video](https://www.youtube.com/watch?v=tJxcKyFMTGo)


## Assignments
1. A pair of prime numbers are called twin primes if they differ by 2, for example (5,7), (11,13) are twin primes. Find and report all twin primes having d decimal digits. You are expected to report the results in myFirstFile.txt file using your code. You can refer to the internet on how to write to a txt file.

   * Ex:

            Input: 1

            Output: A myFirstFile.txt file with first line 3 5 and the second line 5 7

2. Given a palindrome number, find the next smallest palindrome in an efficient way.
    * Ex:
  
            Input: 999                              Input: 121
            Output: 1001                            Output: 131

3. Implement the class of Complex numbers,It should have methods like addition, subtraction, modulus (magnitude), multiplication, conjugate, display and inverse.

   * Ex:
  
        ```python
        a = Complex(1,2) #### a would refer to 1+2*i
        a.display() #### prints out “1 + 2i”
        b = Complex(2,-3)
        c = b.add(a)
        c.display() #### prints out “3 - 1i”
        c.conjugate().display() ### prints “3+1i” 
        ```

4. Write a NumPy program to calculate theta (matrix) using the normal equation.
   $$\theta = (X^TX)^{-1}X^Ty$$
    Where $X$ is any random normalized numpy matrix of shape $(20 \times 20)$, $y$ is a numpy array of length 20 and data type ```int32``` . Look for  ```np.random.normal, np.dtype``` for reference.

5. You are given prices for a particular stock for the next n days, say p1, p2, ....pn. You want to buy one stock on one of the upcoming days and sell it on a later day. Both buying and selling should be done within the next n days. You want to find out which buying and selling days will maximize your profit. If multiple of these options are possible print with the earliest buying date.
   
    Can you think of a very much efficient solution for this?

    Ex:

        The first line of input contains no. of days and the second line contains prices separated by space.
        For the output,The first line prints maximum profit possible. The second line prints the earliest buy date possible such that profit is maximised.
        Input:
        5
        100 10 1110 5000 4000
        Output:
        4990
        2
