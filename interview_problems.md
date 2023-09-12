# PhD Interview Preparation

Welcome to your PhD interview preparation with the Bochum Hadron Physics group. We are eager to learn more about your academic journey and research interests. Before we delve into the interview, we would like you to prepare answers to the following questions. These questions are designed to gauge your understanding and expertise in various crucial aspects of high-energy physics. Please note that you do not need to submit the results of these exercises. Once you are ready, request a call via email to schedule your interview before September 23rd.

During the interview, we will begin with an introduction to our group and the groundbreaking work we are involved in. Following this, you will have the opportunity to introduce yourself and share your academic and research background. The main part of the interview will be a discussion of the exercises outlined below, where you will present your prepared answers. We look forward to a fruitful and engaging discussion with you.

## 1. Master Thesis / Current Work (15')

During your interview, we would like you to discuss a significant aspect of your master thesis / present research. Firstly, please provide a verbal concise explanation of the central problem or research question your thesis addresses. Secondly, select one important plot or figure from your work to discuss in detail.

## 2. Physics Question: Electric Circuit and Resonance Pole (10')

Consider the infinite electric circuit depicted below:

```
...-------------------R-------C-----C-----...
...  |     |     |         |     |     |     
...  L     L     L         C     C     C  ...
...  |     |     |    ~    |     |     |   
...-----L-----L------o o------------------...
```

In this circuit:
- "R" represents a resistor,
- "L" represents an inductor,
- "C" represents a capacitor,
- The "o o" symbol represents an AC voltage source,
- The dots indicate that the pattern of the last (or first) connection cell repeats infinitely.

Your task is to find the resonance pole of this circuit in the complex frequency $\omega$ plane (you should express your answer in terms of R, L, and C, without substituting numerical values). The resonance pole is defined as the point in the complex frequency plane where the impedance of the circuit, becomes zero. Draw a connection with hadron physics resonances.

**Solution format:**
```
\omega_resonance = (function of R,L,C)
\omega_pole = (function of R,L,C)
+ notes, comments
```

**Keywords:** infinite ladder electric circuit, complex frequency domain, resonance poles.

## 3. Statistics Question: Uncertainty for a Bin of Low Statistics (10')

In high-energy physics, counting experiments often involve analyzing data in a histogram to estimate various properties of the system under study including the assessment of counting uncertainty and error estimation. While the square root of the number of counts $\sqrt{N}$ (the Wald approximation) generally offers a good estimation of counting uncertainty, it may not be the most precise approach, particularly for bins with a low number of counts where the probability of observing more counts is higher than observing fewer in repeated experiments, leading to asymmetric uncertainty. For reference, in ROOT, a common tool in high-energy physics, asymmetric errors for low count bins can be enabled using `ROOT.TH1.kPoisson`. The task is to calculate the upper and lower error bars for bins with 5, 50, and 500 counts, aiming for 68.3% central confidence intervals and compare to the Wald approximation.

**Solution format:**
```
  N | Poisson | Wald
---------------------
  5 |  +??-?? |  ±??  
 50 |  +??-?? |  ±??  
500 |  +??-?? |  ±??  
+ notes, comments
```

**Keywords:** counting experiment, probability distribution, confidence interval

## 4. Programming: Charm Hadrons Pie Plots (10')

In this exercise, you are tasked with developing a program using your favorite programming language (Python, Julia, C++, ...) to visualize the quark composition of ground-state charm meson and baryons (D+, D-, Lambda_c+, ...), a category of hadrons containing at least one charm quark (ten hadrons in total). Your goal is to create a series of pie charts (e.g. `ax.pie(..., radius=...)`, or `cis` (math)) where each chart represents a different charm particle, with the area of circle to be proportional to the particle's lifetime. You are expected to consult the [Particle Data Group](https://pdglive.lbl.gov/Viewer.action) (PDG) to collect necessary data on the charm particles, including their names, quark composition, masses, and lifetimes (or use [PDG API](https://pdgapi.lbl.gov/doc/pythonapi.html)). Please push the plotting script to a public GitHub (or any other host) repository, write a short README file on how to run the code.

**Solution format:**
```
Repository: https://github.com/...
```

**Keywords:** constituent quark model, charm hadrons, plotting, version control