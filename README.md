This TIMES-DK model version was developed during the COMETS project for analysing the Danish energy system. Read more about it in an open access article available [here](https://doi.org/10.1016/j.esr.2018.11.003).

The model was used to support climate discussions set out during the summer of 2019. The generated scenarios are shown on https://klimaaftalen2019.tokni.com/

To obtain the model, including the TIMES source code, run the following command:
> git clone --recurse-submodules https://github.com/olejandro/times-dk_gams

To run a specific scenario (e.g. Frozen_policy_scenarie) execute the following command from root:
> GAMS runmodel --comets_scenario=Frozen_policy_scenarie

The model is solved using CBC by default. Adjust the command to solve it e.g., with CPLEX:
> GAMS runmodel --comets_scenario=Frozen_policy_scenarie --solve_with=CPLEX
