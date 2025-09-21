# DICE2023-model-with-carbon-budget-constraint.
A modified version of the GAMS DICE 2023 model with a constraint on the carbon budget (2020-2100) at 1000 GtCO2.

# Modifications
Introduced an additional constraint equation named CONSTCO2EQ for the constraint on the cumulative total carbon emission variable CCATOT
```bash
** declaration
CONSTCO2EQ(t)    Constraint on cumulative total carbon emissions 

**structure of the inequality constraint
constCO2eq(t)..      CCATOT(t) =L= 1000;
