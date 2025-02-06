# How-to-set-up-Python-environments-for-data-projects
My proposal how to set up environment for data projects.

# Python environment issues like conda
TODO:
- pohdi **mambaa**: [a fast, robust, and cross-platform package manager.](https://mamba.readthedocs.io/en/latest/index.html)
- lue dataluminan [VS Code for Data and AI Projects](https://datalumina.clickup.com/docs/9015213037/d/h/8cnjezd-17675/ddd52c673443975)
- Ota käyttöön Data [projektitemplaatti](https://github.com/datalumina/datalumina-project-template)
- Lue [miniconda DS juttu](https://eduand-alvarez.medium.com/setting-up-anaconda-on-your-windows-pc-6e39800c1afb)

# Conda
- [ympäristön hallinta condalla](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)
- 

## oletuspaketit yms ympäristöissä
- [linkki](https://docs.conda.io/projects/conda/en/latest/user-guide/configuration/settings.html#config-add-default-pkgs)

.condarc tiedosto kansiossa `C:\Users\<username>\miniconda3`
- esim `create_default_packages`: Always add packages by default
```yaml
channels:
  - https://repo.anaconda.com/pkgs/main
  - https://repo.anaconda.com/pkgs/r
  - https://repo.anaconda.com/pkgs/msys2

create_default_packages:
  - pip
  - numpy
  - pandas
```


# Conda ympäristön vienti / tallennus
conda env export > name_of_file.yml
ja tuonti, varmista ettei env2 ympäristöä ole olemassa!!!
conda env create -f env2.yml

conda list --export > requirements.txt



# PIP
[Kuinka tarkistaa mitkä papekit asennettu](https://stackoverflow.com/questions/739993/how-do-i-get-a-list-of-locally-installed-python-modules), --local ottaa base, ei ympäristö

```
pip list
pip list --local
```
