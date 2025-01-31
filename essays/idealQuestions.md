---
layout: essay
type: essay
title: "The Importance of Asking Questions in the Right Way" 
# All dates must be YYYY-MM-DD format!
date: 2025-01-30
published: true
labels:
  - Smart Questions
  - Stupid Questions
  - StackOverflow
  - Experience
---

<div class="text-center p-4">
  <img width="500px" src="../img/smartVSstupidQuestion.png" class="img-thumbnail" >
  
</div>



## The Importance of Asking Questions in the Right Way

Asking good questions is important in everyday life. There are many problems that need to be solved—some easier, some more difficult—and sometimes, one may need help to tackle them. Therefore, asking questions in the right way is crucial. When someone asks a question, it becomes evident whether they have actually put effort into solving the problem or if they are simply seeking an easy answer.
There is a phrase my dad used to tell me when I was young: "Having the right questions implies that you are already halfway to solving the problem." In my opinion, he was absolutely right.
Asking the right questions is even more critical for software engineers. [Stack Overflow](https://stackoverflow.com), a question-and-answer website for programmers, is a common place to seek help when stuck on a problem. However, the quality of the question often determines the quality of the response.




## How to Get Help from Stack Overflow When Stuck on a Problem

Understanding what is not working, exhausting all possible options, and doing some research before asking a question are crucial steps to formulating a well-structured inquiry that attracts the attention of those willing to help. The people who answer questions on Stack Overflow can easily see how much effort, time, and research someone has invested in solving a given problem.
A well-formed question should demonstrate an understanding of the problem, an exploration of possible solutions, and clearly state the steps already taken. Additionally, it should be written in proper grammar and spelling to make it easy for others to comprehend.
Consider the following example:


#### [Why is processing a sorted array faster than processing an unsorted array?](https://stackoverflow.com/questions/11828270/how-do-i-exit-vim/11828573#11828573) 

>*In this C++ code, sorting the data (before the timed region) makes the primary loop ~6x faster:* 
>```
>#include <algorithm>
>#include <ctime>
>#include <iostream>
>
>int main()
>{
>   // Generate data
>    const unsigned arraySize = 32768;
>   int data[arraySize];
>
>    for (unsigned c = 0; c < arraySize; ++c)
>        data[c] = std::rand() % 256;
>
>   // !!! With this, the next loop runs faster.
>   std::sort(data, data + arraySize);
>
>    // Test
>    clock_t start = clock();
>   long long sum = 0;
>   for (unsigned i = 0; i < 100000; ++i)
>   {
>        for (unsigned c = 0; c < arraySize; ++c)
>        {   // Primary loop.
>           if (data[c] >= 128)
>                sum += data[c];
>        }
>    }
>
>   double elapsedTime = static_cast<double>(clock()-start) / CLOCKS_PER_SEC;
>
>    std::cout << elapsedTime << '\n';
> std::cout << "sum = " << sum << '\n';
>}
>```
The person not just made a running code, in his question he coded the same program in Javascript as well, to test if the sorthing algorithm depends on the properties of the language, or it is the actual algorithm that is slower/ faster. The question is stated in a way that is really easy to reply to, the code and the question is in a standard, accessible format. The person is precise and informative about his problem, he described the symptoms of the problem or bug carefully and clearly, he "tested" the speed of the algorithm by implementing a function that follows the time. Even though the question and the steps he has taken is fairly long, every information is important, and helpful for the audience of Stackoverflow.  

The response for this clearly stated question was clear, a fairly long, and it was answered in a helpful way, in a "friendly" tone, even  a picture was attached to give a better understanding of the material for the audience. The answer reflects smartness, pateience, time and effort that was put into the answer. 





## How to **NOT** to get an answer 

As mentioned earlier, properly stating a question and demonstrating effort in solving the problem are crucial for receiving a helpful response. The following question, however, does not show any research, effort, or thought:

#### [How do I exit Vim?](https://stackoverflow.com/questions/11828270/how-do-i-exit-vim/11828573#11828573)

>*"I am stuck and cannot escape. It says:"*
>```
>type :quit<Enter> to quit VIM
>```
>*"But when I type that it simply appears in the object body."*


There are several reasons why this is a bad question, as [Eric Raymond](http://www.catb.org/esr/faqs/smart-questions.html) would say:
- The person did not conduct sufficient research before asking.
- They did not check existing forum discussions or manuals that explain basic Vim commands.
- They did not experiment with different solutions before seeking help.

  
Vim has an entire manual dedicated to its usage, and a simple search or reading through the documentation would have answered this question.
Surprisingly, despite the poor quality of the question, the response was still informative. However, as expected, it was much shorter and less detailed than the response to the well-structured question above.

<div >
  <img width="200px" src="../img/sillyQuestion.png" class="img-thumbnail" >
  
</div>


## Conclusion

As an electrical engineer, where coding is also a crucial skill, I learned a lot while reading Raymond’s article and browsing Stack Overflow. A well-formed question—one that demonstrates effort, understanding, and dedication to solving the problem—is far more likely to receive a helpful answer.
Even if the response comes in a rude manner, the knowledge gained from it is still valuable. By asking smart questions, you increase your chances of getting a meaningful answer that helps you understand the problem and its solution better.

