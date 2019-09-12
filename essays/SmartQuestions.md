---
layout: essay
type: essay
title: Stupid Questions do Exist!
# All dates must be YYYY-MM-DD format!
date: 2019-09-12
labels:
  - StackOverflow
---

## Time is Money
Virtually everyone has been in a situation where they try to accomplish a task, something but goes wrong, and they decide to get help. It could be through the internet or through asking someone in person. This is not inherently bad, but the inquirer can end up wasting another person's valuable time depending on the question asked. For instance, going to an online forum and asking "How do I set a static IP address on Windows?" wastes time since consulting the results of a simple web search would yield the solution.

## Methodical vs Mediocre Inquiry
A good question is methodical. They are typically constructive and show that the user has gone through the steps of attempting to troubleshoot the problem themselves, and also lists any relevant factors. Factors such as operating system used, any programs used, any results/outputs, etc. Questions that fall into this category are more likely to be answered and are more likely to generate constructive responses that may lead to a solution. An example of a question that adheres to these points is: "I am trying to connect a Windows 7 machine to the internet. It is connected to a router via ethernet cable and is able to successfully ping the router. The router is connected by ethernet cable to a modem. The modem's internet indicator is lit, however my machine is unable to connect to the internet. What can I try?"

On the other hand, questions that are presented in a vague manner, lack background information, or appear as though the asker did not take any troubleshooting steps prior steps, would deter others form helping. Take for instance the question "How do I add additional attributes to a table?" Disregarding the fact that a Google search could have lead the user to an answer, the question is also lacking information such as what type of database they are using or how they are interfacing with it. The user could even be asking a question about modifying a table on a user interface. Someone answering this question would need more information to construct an accurate reply, if they wanted to.

### Methodical Example
An example of a good question asked on StackOverflow is this one asking about [finding file differences between two Git branches.](https://stackoverflow.com/questions/822811/showing-which-files-have-changed-between-two-revisions) 

The poster concisely states what they want to say when they mention "I want to merge two branches that have been separated for a while and wanted to know which files have been modified." They also mention, link, and talk about an external resource they found and used, showing that they attempted some form of troubleshooting. However, what they found did not quite possess the desired functionality, which led them to starting their StackOverflow post. 

In this scenario, other users answer with the git commands that would accomplish what the poster originally wanted 
`git diff --name-status firstBranch..branchToCompareTo`

## Mediocre Example
This is a StackOverflow question about [a programming error in C++.](https://stackoverflow.com/questions/55690279/error-expected-or-before-numeric-constant)

The poster of this question mentions that there's an error when attempting to compile in their code, "expected ';' ',' or ')'". They also post a small, incomplete segment of their code, shown below:

```cpp
class functions{
  public:
    int m[5];
    int c=0;
    stack_x mem(5);
```

This error be from somewhere else in their code, but they chose not to post all of it. Another user even asked "Where is curly bracket `};` that closes the class declaration?" to which the poster replied "already written but in the very end of the class, i just posted the part which making the error." 

Other users have submitted answers but in both cases the poster replied back saying that neither suggestion fixed their problem. Had the original poster displayed their entire C++ file, other users may have been able to quickly and accurately assess the problem and present a solution. Instead, anyone willing enough to answer this question will have to extrapolate from what little code is available.