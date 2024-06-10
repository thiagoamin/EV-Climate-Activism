<h1 align="center">Expected Value Of Climate Activism</h1>
<h2 align="center">Authors: Thiago Amin and Ruth Ruth Atagbuzia, Daniel Saunder (Supervisor)</h2>
<h2 align="center">Subject: Behavioural Economics</h2>

## 1: Summary

Behavioral economists have long sought to explain the rationality behind participation in collective action. The collective interest model (as cited in Lubell, 2007) is one approach to this issue, but it suffers from flaws: the model leads to counterintuitive predictions, such as the notion that individuals are most likely to participate when the group’s success without them is high, which should undermine the incentive for participation (free-rider issue). Moreover, the model assessment framework suggested by Lubell relies on a limited set of measurement tools, leading to uncertainties in estimating the utilities and probabilities associated with climate change activism. This project develops a revised mathematical version of the collective interest model that provides more intuitive predictions when accouting for the free-rider problem. Although theoretical, we propose a set of statistical tests to evaluate the model's accuracy, using simulated survey data that incorporates new measurements beyond those explored by Lubell, such as generalized social trust and free market value. 

**Figure:** Multidisciplinary Undergraduate Research Conference (MURC) Poster
![Screenshot 2024-05-04 at 9 34 50 PM](https://github.com/thiagoamin/EVClimateActiv/assets/122248078/73b0ffae-9749-4058-9dda-57f632f6518a)

## 2: Introduction
Climate change represents one of the most significant global challenges, necessitating collective action to mitigate its impact. Understanding the factors that motivate individuals to participate in climate activism is crucial for designing effective policies and interventions. This study explores a theoretical model that predicts the expected value of individual participation in climate activism, initially examined by Mark Lubell. The model incorporates several key parameters to estimate the likelihood of participation based on individual and collective incentives.

Lubell's collective interest model is defined by the following equation (Lubell, 2007):

$$
EV(Global Warming Activism) = (p_g \cdot p_i) \cdot V - C + B
$$

where:
- $p_g$ denotes the group’s probability of success,
- $p_i$ represents an individual’s marginal contribution to this probability of success,
- $V$ is the value of the collective public good,
- $C$ refers to the selective costs to the individual,
- $B$ indicates the selective benefits to the individual.

However, several significant issues arise within this model. Firstly, it does not adequately differentiate between success-dependent and success-independent benefits and costs, potentially leading to inaccurate estimations of the overall expected value. Secondly, the definition of the collective public good \( V \) is ambiguous, affecting the model's output based on whether \( V \) is interpreted at an individual or global level. Thirdly, the model’s assumption that agents may act altruistically conflicts with the rational choice theory, which assumes agents act to maximize personal utility.

To address these limitations, we propose an alternative model. In our revised model, the $V$ variable is substituted with two other parameters $B_d$ and $C_d$, and the term $p_g$ is substituted with $1 - p_g$ (see "3: Theorical Comparison"). This new formulation aims to provide a more accurate representation of the dynamics driving individual participation in climate activism.

To compare the effectiveness of these models, we propose using survey data to measure various parameters. The survey questions are designed to capture the expected value of participation, individual influence, probability of group success, benefits, and costs associated with climate activism. These measurements can then be used to estimate the theoretical variables and evaluate the models.

For this comparison, we suggest employing Bayesian statistical methods. By fitting both theoretical models to the survey data and using Bayesian methods, we can estimate the model parameters and employ Bayes factors to determine which model better captures the dynamics of climate activism. This approach allows for a rigorous comparison based on empirical data, enhancing our understanding of the factors influencing individual participation in collective action.

In the following sections, we will detail the theoretical comparison between the two models, propose survey questions to gather the necessary data, and outline the Bayesian approach for model evaluation. This comprehensive examination aims to refine our understanding of the factors influencing climate activism and contribute to the development of more effective strategies for promoting collective action.


## 3: Theoretical Comparison 

Attempting to test a theoretical model that predicts the expected value of participation in climate activism, Lubell evaluated a collective interest model. His multivariable model contains the following parameters: two probability variables which represent the group’s probability of success ($p_g$) and an agent’s marginal contribution to this probability of success ($p_i$); selective costs ($C$) and benefits ($B$) to the individual; and the value of the collective public good $V$. The relationship between these variables is described in the following equation:

<div align="center"><b>M<sub>0</sub> = EV(Global Warming Activism) = [(p<sub>g</sub> × p<sub>i</sub>) × V] - C + B]</sub></b></div>

However, we propose the following alternative model, where the $V$ variable was substituted by two other parameters ($B_a$ and $C_d$), and the term $p_g$ was substituted for $(1-p_g)$:

<div align="center"><b>M<sub>1</sub> = EV(Global Warming Activism) = [p<sub>i</sub>(1 - p<sub>g</sub>)(B<sub>d</sub> - C<sub>d</sub>)] - C<sub>i</sub> + B<sub>i</sub></b></div>

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

## 3: Measurement (Survey Questions)
The following survey questions were designed using Likert scales.
### 3.1: Expected Value of Participation (EV(activism))

- **Outcome Measure Options**:
  - Use a Likert scale to ask about utilities directly.
  - Ask whether respondents take specific actions related to climate change (e.g., participating in protests, membership in activist groups), then use logistic regression to predict the probability of participation.

### 3.2: Individual Influence (Ia or Pi)

- **Question**: "I believe my actions have an influence on global warming and climate change."
  - Scale: 1 (Strongly Disagree) to 5 (Strongly Agree)

### 3.3: Probability of Group Success (Pg)

- **Question 1**: "I am confident that other people are helping to reduce the effects of global warming/climate change."
  - Scale: 1 (Strongly Disagree) to 5 (Strongly Agree)
- **Question 2**: "I believe taking action towards combating global warming/climate change encourages others in my community to take similar steps that increase our energy independence."
  - Scale: 1 (Strongly Disagree) to 5 (Strongly Agree)
- **Question 3**: "I believe that public officials are important in influencing the outcomes of global warming/climate change."
  - Scale: 1 (Strongly Disagree) to 5 (Strongly Agree)

### 3.4 Benefits to the Individual (Bi)

- **Question 1**: "I believe today’s policies must consider the needs of future generations."
  - Scale: 1 (Strongly Disagree) to 5 (Strongly Agree)
- **Question 2**: "Have you talked to friends and family members about global warming/climate change?"
  - Type: True/False

### 3.5 Benefits Dependent on Success (Bd)

- **Question**: "If global warming is happening, to what extent do you believe that it is caused by human activities, as opposed to natural changes in the environment?"
  - Scale: 1 (Strongly Agree) to 5 (Strongly Disagree)

### 3.6 Costs to the Individual (Ci)

- **Question 1**: "What is the highest level of education you have completed?"
  - Type: Ordered scale
- **Question 2**: "What is the estimated annual income for your household?"
  - Type: Real number line
- **Question 3**: "The major cause of increased atmospheric concentration of greenhouse gases is human burning of fossil fuels."
  - Type: True/False

### 3.7 Costs Dependent on Regulation (Cd)

- **Question 1**: "I believe markets should generally be free from government interference and unregulated."
  - Scale: 1 (Strongly Disagree) to 5 (Strongly Agree)
- **Question 2**: "I believe the carbon tax is significantly harmful to the economy."
  - Scale: 1 (Strongly Disagree) to 5 (Strongly Agree)

## 4: Theoretical Model -> Regression Model

### 4.1: Linking Measurements with Theoretical Variables
In each case, we need the appropriate function to convert the units in which a variable is measured to the units in the theoretical model. For instance, \(Pi\) is a probability, ranging from 0 to 1. However, the variable is measured using a Likert scale, which ranges from 1 to 5. To convert this, we consider \(x\) as the Likert score.

#### Probability of Individual Contribution (Pi)
First, we start with a linear regression:
$$Pi = a + bx$$
This linear equation is then transformed into a probability scale using the logistic function, which measures the proportion of the maximum value that the linear regression has traveled across:
$$Pi = \frac{exp(a + bx)}{1 + exp(a + bx)}$$
When the linear regression value is large, the ratio approaches one, and when it is small, the probability approaches zero.

<div align="center">
    <img src="https://github.com/thiagoamin/EV-Climate-Activism/assets/122248078/91f310db-a7e6-491f-84ed-e8d011c9b3b1" width="50%" height="auto">
    <br>
    <b>Figure 3: Relationship between theoretical P_i variable and measured Likert variable</b>
    <br><br>
</div>

#### Probability of Group Success (Pg)
We also have variables that are measured by multiple questions - $p_g$. Therefore, we need a multi-variate regression design.
$$P_g = \frac{exp(a + b_1x_1 + b_2x_2 + b_3x_3)}{1 + exp(a + b_1x_1 + b_2x_2 + b_3x_3)}$$
Each of $(x_1, x_2, x_3)$ are measured using Likert scales.

#### Benefits and Costs
Benefits (Bi) and costs (Ci) in our model are quantified using linear combinations of measured variables. Benefits are defined as $(Bi = a + b_1 \cdot x_1 + b_2 \cdot x_2)$, where $(x_1)$ and $(x_2)$ represent specific Likert scale responses and binary indicators, respectively. Costs are explicitly modeled to incorporate the cumulative impact of various factors such as education level or economic perspectives, defined as $(Ci = a + b_1 \cdot x_1 + b_2 \cdot x_2 + b_3 \cdot x_3$)$.

### 4.2 Complete Regression Model
The complete regression model integrates these variables to estimate the expected value of activism. This model directly connects our actual collected data with our theoretical variables:
$$ev(activism) = \frac{exp(a1 + b1 \cdot x1)}{1 + exp(a1 + b1 \cdot x1)} \cdot (1 - \frac{exp(a2 + b2 \cdot x2 + b3 \cdot x3 + b4 \cdot x4)}{1 + exp(a2 + b2 \cdot x2 + b3 \cdot x3 + b4 \cdot x4)}) \cdot ((a3 + b5 \cdot x5) - (a4 + b6 \cdot x6 + b7 \cdot x7)) + (a5 + b8 \cdot x8 + b9 \cdot x9) - (a6 + b10 \cdot x10 + b11 \cdot x11 + b12 \cdot x12)$$

## 5: Data Simulation and Model Testing
This section outlines the process for evaluating two theoretical models of climate activism—the original Lubell model and our proposed revision—using simulated data. We use Bayesian statistical methods to estimate model parameters and employ Bayes factors to discern which model better captures the dynamics of climate activism.

### 5.1: Simulating Data
We simulate individual data points based on predefined distributions to create realistic datasets for each model structure.
```python
import numpy as np
import pandas as pd
import scipy.stats as stats

def simulate_person():
    pi = stats.uniform().rvs()  # Individual contribution probability
    pg = stats.uniform().rvs()  # Group success probability
    bd = stats.norm(500, 200).rvs()  # Benefits dependent on success
    cd = stats.norm(100, 30).rvs()   # Costs dependent on success
    bi = stats.norm(10, 5).rvs()     # Individual benefits
    ci = stats.norm(50, 20).rvs()    # Individual costs

    ev = pi * pg * (bd - cd) + bi - ci  # Expected value calculation
    return [ev, pi, pg, bd, cd, bi, ci]

# Generate data for 500 simulated individuals
t = [simulate_person() for _ in range(500)]
data = pd.DataFrame(t, columns=['ev', 'pi', 'pg', 'bd', 'cd', 'bi', 'ci'])
```

### 5.2: Model Fitting and Comparison
We fit both theoretical models to the simulated data. The basic idea is to determine model fit using Bayes factors: if the underlying simulation aligns with the Lubell model, it should exhibit a higher Bayes factor compared to our model. Conversely, if our revised model better represents the simulated data, the Lubell model should show a lower Bayes factor.

```python
# Define and fit Lubell's model
with pm.Model() as m0:
    α = pm.Normal('α', 0, 0.5, shape=4)
    β = pm.Normal('β', 0, 0.5, shape=6)
    ϵ = pm.Exponential('ϵ', 1)

    pi = pm.Deterministic('pi', np.exp(α[0] + β[0] * data['pi']) / (1 + np.exp(α[0] + β[0] * data['pi'])))
    pg = pm.Deterministic('pg', np.exp(α[1] + β[1] * data['pg']) / (1 + np.exp(α[1] + β[1] * data['pg'])))
    bd_cd = α[2] + β[2] * data['bd'] + β[3] * data['cd']
    bi_ci = α[3] + β[4] * data['bi'] + β[5] * data['ci']

    μ = pm.Deterministic('μ', pi * pg * bd_cd + bi_ci)
    y_pred = pm.Normal('ev', μ, ϵ, observed=data['ev'])

    trace_m0 = pm.sample(1000)

# Define and fit our revised model
import pymc3 as pm
import arviz as az

with pm.Model() as m1:
    α = pm.Normal('α', 0, 0.5, shape=4)
    β = pm.Normal('β', 0, 0.5, shape=6)
    ϵ = pm.Exponential('ϵ', 1)

    pi = pm.Deterministic('pi', np.exp(α[0] + β[0] * data['pi']) / (1 + np.exp(α[0] + β[0] * data['pi'])))
    pg = pm.Deterministic('pg', np.exp(α[1] + β[1] * data['pg']) / (1 + np.exp(α[1] + β[1] * data['pg'])))
    bd_cd = α[2] + β[2] * data['bd'] + β[3] * data['cd']
    bi_ci = α[3] + β[4] * data['bi'] + β[5] * data['ci']

    μ = pm.Deterministic('μ', pi * (1 - pg) * bd_cd + bi_ci)
    y_pred = pm.Normal('ev', μ, ϵ, observed=data['ev'])

    trace_m1 = pm.sample(1000)

# Compute and compare Bayes factors
comparison = az.compare({'Lubell Model': trace_m0, 'Our Model': trace_m1}, ic='waic')
print(comparison)
```
This integrated approach helps us test theoretical predictions and refine our understanding of participation dynamics in climate activism. By comparing Bayes factors, we can empirically determine which model more accurately reflects the mechanisms driving individual participation in collective action.

## 5: Conclusion
In this project, we explored a theoretical model predicting the expected value of individual participation in climate activism, initially explored by Lubell. While Lubell's model integrates key parameters such as the group's probability of success, individual contribution, and collective public good, it falls short in differentiating between success-dependent and success-independent factors, and it makes counterintuitive predictions regarding rational behavior. To address these issues, we proposed a revised model that substitutes ambiguous variables with more precise ones and incorporates the concept of the free-rider problem. We suggest using survey data to measure the relevant parameters and employing Bayesian statistical methods to compare the models rigorously. This comprehensive approach aims to refine our understanding of the factors driving climate activism and enhance the predictive power and practical application of these theoretical models.

## 5: References
1. Lubell, M., Zahran, S., & Vedlitz, A. (2007). Collective Action and Citizen Responses to Global Warming. Political Behavior, 29(3), 391–413. https://doi.org/10.1007/s11109-006-9025-2
2. Olson, M. (1965). Logic of Collective Action: Public Goods and the Theory of Groups (Harvard economic studies. v. 124). Harvard University Press.
3. Ostrom, E. (1998). A Behavioral Approach to the Rational Choice Theory of Collective Action: Presidential Address, American Political Science Association, 1997. American Political Science Review, 92(01), 1–22. https://doi.org/10.2307/2585925
4. Oliver, P. E. (1993). Formal Models of Collective Action. Annual Review of Sociology, 19, 271–300. http://www.jstor.org/stable/2083389
