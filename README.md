# Uplift Modelling Projects

A portfolio of independent uplift modelling projects: estimating which customers respond to a treatment because of it, from randomised incrementality-test data, and turning those estimates into a targeting policy.

Each project is its own GitHub repository with a reproducible pipeline, offline tests, a notebook, and a README that states its data, method, and limitations.

## Projects

| # | Name | Dataset | Main method | Repository |
|---|------|---------|-------------|-------------|
| 1 | T-Learner Baseline | Criteo uplift benchmark (randomised, 12 anonymised features) | Separate outcome models for treatment and control, scored with the Qini coefficient | [uplift-tlearner-baseline](https://github.com/Patotricks15/uplift-tlearner-baseline) |
| 2 | Class Transformation | Criteo uplift benchmark | Transformed outcome that makes a standard classifier estimate uplift | [uplift-class-transformation](https://github.com/Patotricks15/uplift-class-transformation) |
| 3 | Targeting Policy | Criteo uplift benchmark | Choice of a targeting cutoff from the uplift scores | [uplift-targeting-policy](https://github.com/Patotricks15/uplift-targeting-policy) |

## Status

The notebooks have not been run on the real dataset, so no figures are reported yet. The results will be added after a Kaggle run.

## Key limitations

- The Criteo dataset is listed as CC0 on Kaggle, but the upstream Criteo terms say CC BY-NC-SA 4.0. This conflict is unresolved, so no derived figures are published.
- Uplift is estimated from one randomised test. The estimates hold only for the population and offer in that test.

## Scope

This is part of a 3-repository plan. Projects are added here as they are completed; each repository listed above is self-contained and can be cloned, tested, and run independently.
