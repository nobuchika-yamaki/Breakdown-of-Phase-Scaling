README
Purpose

This code reproduces all simulations and numerical results reported in the manuscript, including trial-level and summary statistics for the critical delay τ₍crit₎.

Main script

run_methods_exact_results.py
Runs all simulations, detects τ₍crit₎ for each trial, and saves results.

Output files

all_trials_taucrit.csv
Trial-level τ₍crit₎ values for all frequencies, models, and trials.

summary_taucrit.csv
Summary statistics with NaN values excluded (mean, std, median, min, max, and f·τ₍crit₎).

Both files are saved to the Desktop.

Models

Delayed phase-oscillator model (Kuramoto-type)

Bilateral Wilson–Cowan excitatory–inhibitory population model

Both models:

use identical delay dynamics,

are integrated with dt = 1 ms,

define synchronization breakdown as |φ_L − φ_R| > 1.8 rad,

match the Methods section exactly.

Execution
python3 run_methods_exact_results.py
