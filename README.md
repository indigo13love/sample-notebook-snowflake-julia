# sample-notebook-snowflake-folium

This is a sample Jupyter Notebook to connect to Snowflake from Julia language, written for https://zenn.dev/indigo13love/articles/7e123bb608ebfb (Japanese article).

To use this notebook, you have to install several Julia and Python packages into Julia:

# Preparation

You have to install `IJulia`, `PyCall`, `DataFrames` and `Pandas` packages, and `snowflake-connector-python` Python package through `pyimport_conda()` in `PyCall`:

```
(@1.5) pkg> add IJulia
...
(@1.5) pkg> add PyCall
...
(@1.5) pkg> add DataFrames
...
(@1.5) pkg> add Pandas
...
julia> using PyCall

julia> pyimport_conda("snowflake.connector", "snowflake-connector-python", "conda-forge")
```
