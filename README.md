# cse344-homework-1---v2-file-i-o-solved
**TO GET THIS SOLUTION VISIT:** [CSE344 Homework #1 – v2 File I/O Solved](https://www.ankitcodinghub.com/product/cse344-homework-1-v2-file-i-o-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;93936&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE344 Homework #1 - v2 File I\/O Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
&nbsp;

</div>
</div>
<div class="layoutArea">
<div class="column">
The goal is to develop a simple text editor accomplishing a common task: string replacement. It must support the following:

a) ./hw1 ‘/str1/str2/‘ inputFilePath

This will replace all occurrences of str1 with str2 in the file inputFilePath (relative or absolute)

b) ./hw1 ‘/str1/str2/i‘ inputFilePath

This will perform the same as before, but will be case insensitive.

c) ./hw1 ‘/str1/str2/i;/str3/str4/‘ inputFilePath It must be able to support multiple replacement operations.

d) ./hw1 ‘/[zs]tr1/str2/‘ inputFilePath

It must support multiple character matching; e.g. this will match both ztr1 and str1

e) ./hw1 ‘/^str1/str2/‘ inputFilePath

It must support matching at line starts; e.g. this will only match lines starting with str1

f) ./hw1 ‘/str1$/str2/‘ inputFilePath

It must support matching at line ends; e.g. this will only match lines ending with str1

g) ./hw1 ‘/st*r1/str2/‘ inputFilePath

It must support zero or more repetitions of characters; e.g. this will match sr1, str1, sttr1, sttttr1, etc

And of course it must support arbitrary combinations of the above;

e.g. ./hw1 ‘/^Window[sz]*/Linux/i;/close[dD]$/open/‘ inputFilePath

Assume that the user will try to match/replace only letters and digits, but no symbols or space. Hence you will not need escape characters.

Output

The output will be written to the input file. If you need temporary files, you must use mkstemp().

Is this all?

No. The program might be executed as multiple instances with different replacement commands, on the same file. This will result in multiple processes manipulating the same input file with potentially wrong results.

Imagine for instance one process replacing str1 with str2, and another replacing str2 with str3 at the same time. Depending on which process writes/reads what, the end result might vary. You cannot stop the user from invoking your program multiple times, so instead you must protect file access (via the locks seen during our lectures) by making sure than no second instance of the program runs on the same file, before the first one has finished its task with it.

For all file I/O operations, use the low-level system calls presented during our lecture and not C library functions. Make sure you control each system call’s return value and print informative

</div>
</div>
<div class="layoutArea">
<div class="column">
March 10th, 2022

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
messages via perror/strerror in case of errors. Make sure you print your program’s usage in case the commandline arguments are wrong.

</div>
</div>
</div>
