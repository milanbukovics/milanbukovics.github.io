---
layout: essay
type: essay
title: "The importance of asking questions in the right way" 
# All dates must be YYYY-MM-DD format!
date: 2025-01-30
published: true
labels:
  - Smart Questions
  - Stupid Questions
  - StackOverflow
  - Experience
---

## The importance of asking questions in the right way

Asking a good question is important in the everyday life. There are many pronlems that has to be solved, some of them are easier, some of them 
are more difficult, and one may need some help to tackle these problems. Therefore, asking questions in the right way is crucial; if someone ask a question, then from that it can
be easily decided if the person actually put effort into trying to solve the problem, or he/she did not. There is a phrase that I was told by my Dad when I was youg that "Having the right questions implies that you are already halfway to solve the problem", and in my opinion he is right. 

Asking the right questions applies even more for software engineers. [Stackoverflow](https://stackoverflow.com), a question-and-answer website for keyboard warriors, is a common placce to ask questions and get informed in case someone is stuck with a problem.


## How to get help from Stackoverflow in case we are stuck with a problem

Understanding what is not working, exploiting majority of the options to find the answer, do some digging to get to the solution is crucial to state the right question, and to get the attention of those who are willing to answer. These people who answer questions on Stackoverflow can easily see how much effort, time, and researh one invested into solving the given problem. The following question shows understanding of the problem, exploaration majority of the possible solutions, and the question and the steps that have been already taken, are written in clear, grammatical, correctly-spelled language.


[Why is processing a sorted array faster than processing an unsorted array?](https://stackoverflow.com/questions/11828270/how-do-i-exit-vim/11828573#11828573) 
*In this C++ code, sorting the data (before the timed region) makes the primary loop ~6x faster:* 
```
#include <algorithm>
#include <ctime>
#include <iostream>

int main()
{
    // Generate data
    const unsigned arraySize = 32768;
    int data[arraySize];

    for (unsigned c = 0; c < arraySize; ++c)
        data[c] = std::rand() % 256;

    // !!! With this, the next loop runs faster.
    std::sort(data, data + arraySize);

    // Test
    clock_t start = clock();
    long long sum = 0;
    for (unsigned i = 0; i < 100000; ++i)
    {
        for (unsigned c = 0; c < arraySize; ++c)
        {   // Primary loop.
            if (data[c] >= 128)
                sum += data[c];
        }
    }

    double elapsedTime = static_cast<double>(clock()-start) / CLOCKS_PER_SEC;

    std::cout << elapsedTime << '\n';
    std::cout << "sum = " << sum << '\n';
}
```
The person not just made a running code, in his question he coded the same program in Javascript as well, to test if the sorthing algorithm depends on the properties of the language, or it is the actual algorithm that is slower/ faster. The question is stated in a way that is really easy to reply to, the code and the question is in a standard, accessible format. The person is precise and informative about his problem, he described the symptoms of the problem or bug carefully and clearly, he "tested" the speed of the algorithm by implementing a function that follows the time. Even though the question and the steps he has taken is fairly long, every information is important, and helpful for the audience of Stackoverflow.  

The response for this clearly stated question was clear, a fairly long, and it was answered in a helpful way, in a "friendly" tone, even  a picture was attached to give a better understanding of the material for the audience. The answer reflects smartness, pateience, time and effort that was put into the answer. 





## How to **NOT** to get an answer 

As it was mentioned above, the right way of stating the question, and showing that there is actually tear and sweat to get to the answer is crucial. The following question does not demonstrate time investment, nor effort, no nothing into the following question: 


### [How do I exit Vim?](https://stackoverflow.com/questions/11828270/how-do-i-exit-vim/11828573#11828573)

*I am stuck and cannot escape. It says:*
```
type :quit<Enter> to quit VIM
```
*But when I type that it simply appears in the object body.*

There are multiple reason this question is a "Stupid question", as [Raymond](http://www.catb.org/esr/faqs/smart-questions.html) would say: It can be seen here that the research
wasn't deep enough to solve this question. The archives of the forum or mailing list the person posted clearly wasn't read, nor researched, the experimentation of getting to the solution is not sufficient. Furthermore, there is a whole manual dedicated to use the command line, bash. It includes the basic text editors, such as *VIM* or *NANO*. 

Surprisingly, the answer turned out to be surprisingly informative, even though "stupid questions" tend to be disregarded or answered in a really short sentence. The answer wasn't as long as it was at the previous question, as expected, but it is still informative. 

## Conclusion

As an electrical engineer, where coding is also really important, I learned a lot as I was reading Raymond's artcile and browsing through Stackoverflow. A clearly stated question, that shows that the person is invested into the problem, shows undestanding of the problem and dedication to solve it, should give you an answer in the end. From the answer, you will realize what did you not check out, or clears up some confusion. At the end of the day though, you gained knowledge, even if the response is in a rude manner. 


