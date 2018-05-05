# linguistic-intelligence

A goal-driven reinforcement learning using the communication channel with new auto-made, auto-changing, and non-human languages. 

<br>

## Hypothesis

Actual language understanding will come from agents that learn words in combination with how they affect the environment effectively, rather than spotting patterns in a huge corpus of text.

#### What is an agent?

An agent can be a network system, a chatbot, an AI, a compiler et cetra.

### Relating Language to maximum goal-driven utility.

Language is one of multiple tools which an agent may use to accomplish goals in its environment and can use to perform the maximum utility in an enviornment. By understanding a part of language we mean it is able to use language productively to accomplish these goals. Under this definition, an agent’s communication success reduces to its success on tasks within its environment.


### Using Reinforcement Learning

Possibly the idea is to get them to creating their own form of language by dropping them into a set of simple worlds, giving them the ability to communicate, and then giving them goals that can be best achieved by communicating with other agents. If they achieve a goal, then they get rewarded. We train them using reinforcement learning and, also making sure that they develop a shared language to help them achieve their goals.

<br>

## Problem

It can be represented as a _**'Cooperative or Competitive Multi-Agent Reinforcement Learning'**_. 

<br>

## Theoretical-Approach


### Work For an Agent

- Each named agent exist in a defined environment and each agent has a goal, a specific work to do. 
- Each agent can broadcast messages to the group as a whole and can broadcast message privately. 
- Every agent's reward is the sum of the rewards paid out to all agents, encouraging collaboration as well as competitiveness, with the main goal is to complete the given task as soon as it can.

### What should be some constraints?

- Before an agent takes an action it will first observes the communications with others privately as well as publicly, now as soon as the surety level of an agent to take an action increases upto a certain level it starts doing its work.

- An agent will store the communications and the result of the action in a private recurrent neural network, giving it a memory or an experience for the word it hears in the form of its new language.

### Making Use of Communication Channel.

It will make use of a some messages (formed in its own language) sent over a differentiable communication channel i.e. it allows agents to directly inform each other about what message they have sent at each time span. We can add a certain reward if the message brings a positive change in completing the work given to that agent, possibly calculates as the differentiation of the future reward with respect to the changes in the sent messages.

- Any agent can send the messages in the way of discrete set of vector of real/binary numbers or a continous stream of approximated binary numbers. If we use the approximate discrete communication of a set of approximated binary numbers it will be probably more easy to interpret.

- Any agent will be rewarded when it will use the communication channel to achieve a task quickly.

- Any agent will be rewarded for speaking a particular word invented in their own language that is proportional to how frequently that word has been spoken previously.

<br>

## Further Research

- We can simultaneously introduce more than 3 agents that should cooperate with themselves to achieve some set of goals, in which 2 agents will try to use the communication channel with their own language and the third try to use basic semantics of human language and the data that the agents learn to acheive the goals can be used to train a neural network which at some level can be used as an algorithm which is linked between the two different languages.

