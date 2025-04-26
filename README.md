# cs-7642-homework-3-reinforcement-learning-and-decision-making-solved
**TO GET THIS SOLUTION VISIT:** [CS 7642: Homework #3 Reinforcement Learning and Decision Making Solved](https://www.ankitcodinghub.com/product/cs-7642-reinforcement-learning-and-decision-making-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;105387&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS 7642: Homework #3 Reinforcement Learning and Decision Making Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
SARSA Homework #3

1 Problem

1.1 Description

For this assignment, you will build a SARSA agent which will learn policies in the OpenAI Gym Frozen Lake environment. You will be given randomized Frozen Lake maps, with corresponding sets of parameters to train your SARSA agent; if your agent is implemented correctly, after training for the specified number of episodes it will produce the same policies (which are not necessarily optimal policies) as the grader.

Frozen Lake is a grid world environment that is highly stochastic, where the agent must cross a slippery frozen lake which has deadly holes to fall through. The agent begins in the starting state S and is given a reward of 1 if it reaches the goal state G. The agent can take one of four possible moves at each state (left, down, right, or up). The frozen cells F are slippery, so the agent’s actions succeed only of the time, while the other are split evenly in orthogonal directions. If the agent lands in a hole H, then the episode terminates, and the agent is given a reward of 0.

Figure 1: Example Frozen Lake Map

1.2 SARSA (st,at,rt+1,st+1,at+1)

SARSA is a model-free on-policy reinforcement learning algorithm that solves the control problem through trial-and-error learning. It is model-free because, unlike with value iteration and policy iteration, it does not need or use an MDP. It is on-policy because it learns about the same policy that generates behaviors. The algorithm estimates the action-value function Qπ of the behavior policy π, and uses an exploration strategy to improve π while increasing the policy’s greediness.

1.3 Procedure

1. Install OpenAI Gym 0.14.0 with pip install gym==0.14.0

2. Implement a SARSA agent

3. Train your agent given the specified parameters

4. Export the policy and enter it into Canvas

1.4 Notes

• You must use Python, NumPy, and OpenAI Gym 0.14.0 for this homework • Use the provided seed for both Gym and NumPy

1

–SARSA 2

• Initialize the agent’s Q-table to zeros

• To avoid any unexpected behavior, setup the Gym environment with gym.envs.toy text.frozen lake.FrozenLakeEnv().unwrapped

• To set up the environment with a custom map, use the environment’s desc attribute. Note that the environment expects a square map so you will need to reshape it.

• You must train your agent with an epsilon-greedy exploration strategy, using NumPy’s numpy.random.randint function to select random actions

1.5 Examples

The following examples can be used to verify that your agent is implemented correctly.

• Input: amap=’SFFFHFFFFFFFFFFG’, gamma=1.0, alpha=0.25, epsilon=0.29, n episodes=14697, seed=741684, Output:

∧,∨,∨,&gt;,&lt;,&gt;,&gt;,∨,∨,∨,&gt;,∨,&gt;,&gt;,&gt;,&lt;

• Input: amap=’SFFFFHFFFFFFFFFFFFFFFFFFG’, gamma=0.91, alpha=0.12, epsilon=0.13, n episodes=42271, seed=983459, Output:

∧,&gt;,&gt;,&gt;,&gt;,&lt;,&gt;,&gt;,&gt;,∨,∨,∨,&gt;,&gt;,∨,∨,&gt;,&gt;,&gt;,&gt;,∨,&gt;,&gt;,∧,&lt;

• Input: amap=’SFFG’, gamma=1.0, alpha=0.24, epsilon=0.09, n episodes=49553, seed=202404, Output:

&lt;,&lt;,∨,&lt;

1.6 Resources

1.6.1 Lectures

• Lesson 4: Convergence

1.6.2 Readings

• Chapter 6 (6.4 Sarsa: On-policy TD Control) of Sutton and Barto 2018

1.7 Submission Details

References

[SB18] Richard S Sutton and Andrew G Barto. Reinforcement learning: An introduction. MIT press, 2018.
