# Neural manifold under plasticity in a goal driven learning behaviour

Computational investigation of interplay between the low-dimensional dynamics of a recurrent neural network and plastic recurrent weight changes.

Corresponding paper: [Feulner and Clopath, 2021](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1008621).

Requires Python 3.

# Setup python environment

python 3.9.12 and pip 21.2.4

```bash
# create python virtual environment
python -m venv manifold_env

# activate environment
source manifold_env/bin/activate

# install dependencies
pip install -r requirements.txt
```

# Run scripts

## Figure 2

Move to the clone directory (e.g., in my home directory):

```bash
cd ~/neural-manifold-and-plasticity/
```

Run simulation (takes 10 min):

```bash
python fig2_simulation.py
```

The script creates simulation files stored in data/fig2/:

```
- data/
    fig2/
        experiment_results.npy
        network.npz
        relearning_results.npy
        W_initial.npy
        W_outside.npy
        W_stabilized.npy
        W_within.npy
```

Reproduce figure 2 (.svg files stored in figures/fig2/):

```bash
python fig2_plots.py
```

## Figure 3

run simulation figure 3 (takes 10 min):

```bash
python fig3_simulation.py
```

Reproduce figure 3 (.svg files stored in figures/fig4/):

```bash
python fig3_plots.py
```

## Figure 4

Run simulation for figure 4 (takes 10 min):

```bash
python fig4_simulation.py
```

Reproduce figure 4 (.svg files stored in figures/fig4/):

```bash
python fig4_plots.py
```

etc ...