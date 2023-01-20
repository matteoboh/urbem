# UrbEm

Urban data analysis of vehicle emissions.
 
Urban emissions represent a major antagonist to cities' livability. In this work, we investigate vehicle emissions using both spatial and non-spatial models to study their relationships with a variety of urban features. We compare such models in terms of performance and interpretation, showing not only that a spatial model has better performances, but also that it is very powerful in explaining the roles played by the predictors in different areas of the city. In particular, we find that the CO$_2$ emissions in the city of Rome are mainly correlated with the presence of main arterial roads, but also to the population density, and to the road network density in general. Moreover, the importance of such factors changes within different areas of the city. While being an experimental proof of spatial regression's efficacy when modelling urban emissions, our work may also help in understanding the complicated relationships between the urban environment and the spatial variability of vehicle emissions in the city of Rome.

---

## Development Setup

```sh
# Create conda environment, install dependencies on it and activate it
conda env create --name urbem --file environment.yml
conda activate urbem

# Setup pre-commit and pre-push hooks
pre-commit install -t pre-commit
pre-commit install -t pre-push
```

## Update dependencies

To add new dependencies or to update existing ones:

1. Add the name (and version if needed) to the list of dependencies in `environment.yml`
2. run `conda env update --name urbem --file environment.yml  --prune`
3. Update the file `environment.lock.yml` by running `conda env export > environment.lock.yml`

## Credits

This package was created with the [BSCCNS/cookiecutter-data-science](https://github.com/BSCCNS/cookiecutter-data-science) project template.
