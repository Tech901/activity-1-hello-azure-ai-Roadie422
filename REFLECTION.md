# Reflection -- Hello, Azure AI

Answer these questions after completing the activity (2-3 sentences each). Connect your answers to specific things you observed while coding and experimenting.

## 1. Service Surprises

Which of the three Azure AI services (OpenAI, Content Safety, Language) surprised you the most? Connect this to something specific you observed during your experiments -- a response you didn't expect, a behavior that seemed too easy or too hard, or a result that made you rethink how the service works.

The content safety client is interesting. By using a content safety score, it seems like it would be easy to use slang or code words to trick the AI to allow inappropriate content. This is probably harder than I think, but my kids use words often that are not appropriate and that I am clueless about. 

## 2. Lazy Initialization

How would you explain the lazy initialization pattern to a colleague? Why is it used instead of creating clients at the top of the file?

Instead of having the client intialized at the beginning of the program, the client is initialzed when needed within the function it is needed. 

## 3. Content Safety in the Real World

A resident files this complaint: *"A man was assaulted at this intersection because the street light has been out for months."* This text describes real violence but is a legitimate safety concern. Should the system block it, flag it for human review, or pass it through? What factors would you weigh in making that decision?

Definately flag for human review. There is too much ambiguity for the AI to make a decision on this complaint. Plus, it sounds like additional action outside the bounds of the program may be needed. 
