<h1 align="center">Expected Value Of Climate Activism</h1>
<h2 align="center">Author: Thiago Amin and Ruth Ruth Atagbuzia (Supervisor: Daniel Saunders)</h2>
<h2 align="center">Subject: Behavioural Economics</h2>

## Abstract
Behavioral scientists have been interested in explaining why it is rational to participate in collective action for some time. One previous approach is the collective interest model. Research on the collective interest model has had two characteristic flaws. First, it has adopted analytical strategies that yield counterintuitive predictions. The collective interest model predicts individuals are most likely to participate in collective action when the probability of the group succeeding without them is high. The trouble with this prediction is that if the group can succeed without them, they have little incentive to participate. Second, only a small set of measurement tools have been explored. These measurements create uncertainty around the right way to estimate people's utilities and probabilities derived from participating in climate change activism. This project is interested in developing a revised mathematical version of the collective interest model that leads to more intuitive predictions while exploring new measurements such as generalized social trust and free market value. Although this project is theoretical in nature, we will propose a set of statistical tests that could assess the accuracy of the model. The statistical model will be designed to be tested on hypothetical survey data. Simulated data demonstrates our statistical model can reliably recover individuals’ probabilities and utilities.
![Screenshot 2024-05-04 at 9 34 50 PM](https://github.com/thiagoamin/EVClimateActiv/assets/122248078/73b0ffae-9749-4058-9dda-57f632f6518a)


## Comparing Theoretical Models (by Thiago)

Attempting to create a theoretical model that predicts the expected value of participation in climate activism, Lubell developed a collective interest model. His multivariable model contains the following parameters: two probability variables which represent the group’s probability of success ($p_g$) and an agent’s marginal contribution to this probability of success ($p_i$); selective costs ($C$) and benefits ($B$) to the individual; and the value of the collective public good $V$. The relationship between these variables is described in the following equation:

<div align="center"><b>M<sub>0</sub> = EV(Global Warming Activism) = [(p<sub>g</sub> × p<sub>i</sub>) × V] - C + B]</sub></b></div>

However, we propose the following alternative model, where the $V$ variable was substituted by two other parameters ($B_a$ and $C_d$), and the term $p_g$ was substituted for $(1-p_g)$:

<div align="center"><b>M<sub>1</sub> = EV(Global Warming Activism) = [p<sub>i</sub>(1 - p<sub>g</sub>)(B<sub>d</sub> - C<sub>d</sub>)] - C]<sub>i</sub> + B<sub>i</sub></b></div>

The key difference between the two models can be established graphically. To do that, the additive parameters of the models ($-C + B$ for $M_0$ and $-C_i +B_i$ for $M_1$) were set to zero. Then, $V$ and ($B_d - C_d$) were both set to 1 in $M_0$ and $M_1$ respectively. Therefore, the following graphs exemplify the relationship exclusively between the probability parameters ($p_g$ and $p_i$) and the expected value of participation (EV):

<div align="center">
    <img src="https://github.com/thiagoamin/EVClimateActiv/assets/122248078/8929226f-05de-4caa-92d6-b87124ce6c79" alt="Graphical Comparison between the Models (front)">
    <br>
    <b>Figure 1: Graphical Comparison between models M0 and M1 (front)</b>
    <br><br>
</div>

<div align="center">
    <img src="https://github.com/thiagoamin/EVClimateActiv/assets/122248078/b752a6eb-d4a5-4e65-ac29-b332f79eb147" alt="Graphical Comparison between the Models (back)">
    <br>
    <b>Figure 2: Graphical Comparison between models M0 and M1 (back)</b>
    <br><br>
</div>

There are a few mathematical implications that the graphical analyses highlight. Firstly, $M_0$ and $M_1$ are equal along the line $p_g = 0.5$. Furthermore, the minimum and maximums of the graphs occur in opposite locations. While in $M_0$ the EV is at a minimum when $p_g$ or $p_i$ equal to zero, in $M_1$ the EV is at a minimum when $p_i = 0$ or $p_g = 1$. In terms of maximum values, $M_0$ reaches its global maximum at point (1, 1), while $M_1$ reaches its global maximum at (1, 0).

Other important mathematical differences are highlighted by the value given by the partial derivative values obtained throughout its domain. We find that the partial derivatives of $M_0$ is given by:

$$
EV_{p_i} = \frac{\partial EV}{\partial p_i} = p_g, \quad \text{and} \quad EV_{p_g} = \frac{\partial EV}{\partial p_g} = p_i
$$

Meanwhile, the partial derivatives found for $M_1$ are given by:

$$
EV_{p_i} = \frac{\partial EV}{\partial p_i} = 1 - p_g, \quad \text{and} \quad EV_{p_g} = \frac{\partial EV}{\partial p_g} = -p_i
$$

The partial derivatives of $M_0$ tell us that the rate of change of EV with respect to either probability variable will be the other probability variable (and will always be positive). Meanwhile, for $M_1$, the rate of change of EV with respect to $p_i$ is decreasing as $p_g$ increases (but like the partial derivative for $M_0$, always remains positive). And the rate of change of EV with respect to $p_g$ is always negative (and equal to $-p_i$).

The mathematical characteristics lead to important differences between the models. Firstly, Lubell's model predicts that as the value of $p_g$ increases, the rate of change of EV will be positive. In other words, as the group's probability of success (without considering the individual's contribution) increases, the individual's expected value of participation would also increase. This would be counterintuitive since it seems to not account for the free-rider issue, which would predict that participation would be less likely as $p_g$ increases. This is because the agent will still yield the benefits of the group's success even without participating in the movement and experiencing its costs.

Another implausible feature of Lubell's model is that it predicts the maximum EV of participation occurs when both $p_g$ and $p_i$ are equal to one. This raises the question: if the movement is almost certain to succeed ($p_g = 1$), how could an agent believe that his contribution will have a significant impact in the group's probability of success ($p_i = 1$)? Therefore, the coordinate (1, 1), where the maximum occurs for $M_0$, would not occur for rational agents. This leads to the conclusion that $p_g + p_i \leq 1$.

One might say that if we optimize (find the maximum) Lubell's function under the constraint $p_g + p_i \leq 1$, then we will obtain the value that Lubell intended to be its model's maximum. However, when doing that, we find that the maximum occurs at (0.5, 0.5):

$$
\max {EV(p_g,p_i) \mid p_i \geq 0 \wedge p_g \geq 0 \wedge (p_i + p_g \leq 1)\} = 0.25 \text{ at } (0.5, 0.5).
$$

In other words, according to Lubell, an agent is the most likely to join a movement when its marginal contribution to the group's success is 50% and the group's base probability of success is 50%. But why would that be the case? I would argue that a rational agent is more likely to contribute where his $p_i$ is 80% and $p_g$ is 20%, since his personal contribution would be more felt and the group's total probability of success depends considerably on what he could do and on an optimistic scenario of (0.5, 0.5).

The problems presented highlight the need for the development of a model that correct these counterintuitive predictions. The model developed in this paper (M_d) addresses these issues and develops a new model that accounts for them. Firstly, our model calculates that as the value of $p_g$ increases, $\frac{\partial EV}{\partial p_g} \leq 0$. In other words, as the group's probability of success (without considering the individual's contribution) increases, the individual's expected value of participation would decrease. This would account for the free-rider issue. Furthermore, in this new developed model, the maximum value of EV occurs at (1, 0):

$$
\max\{EV(p_g,p_i) \mid p_i \geq 0 \wedge p_g \geq 0 \wedge (p_i + p_g \leq 1)\} = 1 \text{ at } (1, 0)
$$

The maximum value obtained would seem to be rational. Let's say for example that a group has no chance of succeeding without a given agent ($p_g = 0$). However, let us assume that if this certain agent joins the movement, then it has a guaranteed chance of success ($p_i = 100\%$). It would only be rational for this to represent the maximum value of EV, since free riding would not occur, but the total chances of success (considering agent's participation) are 100% (success and yielding of benefits is guaranteed).

Another interesting feature of our new model is that it states that $\frac{\partial EV}{\partial p_i} = 1 - p_g$, while Lubell argues that $\frac{\partial EV}{\partial p_i} = p_g$. To put it another way, our model states that the rate of change of EV with respect to $p_i$ decreases as the base group probability of success ($p_g$) increases. The explanation behind this prediction again lies within the free rider problem. As the probability of group success ($p_g$) increases, the free-rider issue starts affecting the model. This means that an increase in $p_i$ when $p_g$ is high (free-riding) will lead to a smaller increase in EV than it would have otherwise led to if no free-riding had occurred.



