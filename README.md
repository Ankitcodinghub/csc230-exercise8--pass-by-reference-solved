# csc230-exercise8--pass-by-reference-solved
**TO GET THIS SOLUTION VISIT:** [CSC230 Exercise8- Pass By Reference Solved](https://www.ankitcodinghub.com/product/csc230-exercise8-pass-by-reference-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;62721&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSC230 Exercise8- Pass By Reference Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 0px;">
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
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<strong>Pass By Reference </strong>

This exercise will give you a chance to work with pass-by-reference, one of the first, useful things we can do with pointers.&nbsp; On the course homepage you will find a partial implementation called passByReference.c. You can also download a copy of

curl -O https://www.csc2.ncsu.edu/courses/csc230/exercise/exercise08/passByReference.c curl -O https://www.csc2.ncsu.edu/courses/csc230/exercise/exercise08/expected.txt

The program won’t compile until you add a few missing functions.&nbsp; Once it’s working, it should print the following output when run:

a = 100 b = 50 c = 25 a = 110 b = 60 c = 35 a = 60 b = 35 c = 110 a = 60 b = 35 c = 109

From the source code, you’ll see you have to add three functions.&nbsp; You can’t modify the contents of main() at all, but by taking parameters passed by address (and maybe some passed by value also), your three functions will be able to change the contents of variables declared in main.

Here’s what your functions need to do:

&nbsp;

<ul>
<li><strong>incrementAll( )</strong> : This function will take pointers to a, b and c and a 4<sup>th</sup> integer parameter. Its job is to increment a, b and c by the value of the 4<sup>th</sup>&nbsp; The main( ) function uses this to add 10 to each of the variables.</li>
<li><strong>rotate( )</strong> : This function will take pointers to a, b and c. Its job is to simultaneously copy the value of&nbsp; b to a, c to b and a to c.&nbsp; You’ll probably want to use a temporary, local variable in the rotate() function to hold the integer value one of the parameters points to while you’re moving values around.</li>
<li><strong>getLargest( )</strong> : This function will take the addresses of a, b and c and it will return the address of the one containing the largest value. So, you’ll be creating a function that returns a pointer.</li>
</ul>
&nbsp;

We looked at an example of return-by-address in class.&nbsp; You need to give <strong>int *</strong> as your function’s return type (to return a pointer to int).&nbsp; Inside your function, you’ll need to compare the values your three parameters point to, and figure out which is the largest.&nbsp; Then, you’ll need to return a copy of the pointer that points to the largest one.&nbsp; Since your parameters are already pointers to ints, you can just return a copy one of your parameters.&nbsp; If you find yourself trying to use the address-of operator here, you’re probably making a mistake.

&nbsp;

Your program should guarantee that the functions will not modify <u>the pointers</u> (e.g., the pointer to a should not be modified to point to b instead) that are passed to them (hint: use the const qualifier to ensure this).

&nbsp;

When you’re done submit your completed passByReference.c file to the exercise_08 assignment in Moodle.
