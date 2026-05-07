# Social Foraging in a Networking Event

This project was created as part of the final work for **NEUR1660: Neural Computation in Decision Making** at **Brown University**.

**Authors**: Aida Abkenova, Ellie Jeong, Viraj Nautiyal

## Background

Optimal foraging theory predicts how an agent should allocate limited time across “patches” to maximize reward, balancing gains against costs. A core result is **Charnov’s Marginal Value Theorem (MVT)**: leave a patch when its current reward rate falls below the environment-wide average.

Patch-leaving also has a well-studied neural signature (e.g., dACC ramping with depletion), which connects naturally to the **drift diffusion model (DDM)**: a decision variable accumulates noisy evidence over time until it reaches a threshold and triggers a switch.

Classical foraging models were developed for asocial environments, but **social foraging** emphasizes that payoffs can depend on social structure and other agents. Here, we apply single-agent foraging ideas to a social setting by framing a **job-search networking event** as a patch-leaving problem: each conversation partner is a discrete “patch” with a hidden binary resource (whether they can offer a job lead), and conversational cues provide noisy evidence about that hidden state. We then compare patch-leaving strategies (including MVT- and DDM-inspired rules) for how a networker should allocate time across conversations.

## Project structure

```text
social-foraging/
  NEUR1660_final.ipynb    # simulation + analysis notebook
  figures/               # exported figures and animations used in the writeup
  README.md
```

## Figures

### Agent illustrations

![Control agent (Figure A)](figures/control%20agent%20(Figure%20A).png)
![MVT agent (Figure B)](figures/MVT%20agent%20(Figure%20B).png)
![DDM Agent (Figure C)](figures/DDM%20Agent%20(Figure%20C).png)
![Epsilon greedy agent (Figure D)](figures/epsilon%20greedy%20agent%20(Figure%20D).png)

### Results snapshots

![Distribution](figures/fig1_distribution.png)
![By environment](figures/fig2_by_environment.png)
![DDM vs MVT](figures/fig3_ddm_vs_mvt.png)
![DDM residence](figures/fig4_ddm_residence.png)
![Residence (all agents)](figures/fig5_residence_all_agents.png)
![Parameter sensitivity](figures/fig6_param_sensitivity.png)
![Efficiency](figures/fig7_efficiency.png)
![Cumulative](figures/fig8_cumulative.png)

### Animations (examples)

![Baseline animation](figures/animation_baseline_best.gif)
![MVT animation](figures/animation_mvt_best.gif)
![DDM animation](figures/animation_ddm_best.gif)
![Epsilon-greedy animation](figures/animation_epsilon_greedy_best.gif)

## What’s in this repo

- `NEUR1660_final.ipynb`: simulation and analysis notebook (environment setup, condition sweeps, and results).

## Citations

- Charnov, E. L. (1976). Optimal foraging, the marginal value theorem. *Theoretical Population Biology*.
- Giraldeau, L.-A., & Caraco, T. (2000). *Social Foraging Theory*. Princeton University Press.
- Hayden, B. Y., Pearson, J. M., & Platt, M. L. (2011). Neuronal basis of sequential foraging decisions in a patchy environment. *Nature Neuroscience*.
- Blanchard, T. C., & Hayden, B. Y. (2022). [Work on foraging/patch-leaving and cingulate cortex]. *(see course/readings for full citation)*.
- Gabay, A. S., & Apps, M. A. J. (2021). [Work connecting foraging frameworks to social decision-making]. *(see course/readings for full citation)*.



