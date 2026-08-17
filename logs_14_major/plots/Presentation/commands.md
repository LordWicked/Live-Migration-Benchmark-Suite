# Main Comparison
.venv/bin/python Scripts/plot_throughput.py \
  logs_14_major/Precopy_Convergent \
  --plots throughput \
  --baseline-dir logs_14_major/Baseline_4T \
  --no-iqr \
  --compact-legend \
  --baseline-color '0.65' \
  --no-timing-note \
  --shade-migration-phase \
  --omit-incomplete-median-tail \
  --title '' \
  --x-label '' \
  --y-label '' \
  --font-size 22 \
  --x-range 125 225 \
  --y-range 0 2250 \
  --x-tick-step 25 \
  --output /tmp/Main-Precopy.pdf \
  --median-output logs_14_major/plots/Presentation/Main-Precopy.pdf \
  --main-line-width 3.5 \
  --baseline-line-width 2.5 \
  --event-line-width 3.0

.venv/bin/python Scripts/plot_throughput.py \
  logs_14_major/Postcopy_4T \
  --plots throughput \
  --baseline-dir logs_14_major/Baseline_4T \
  --no-iqr \
  --compact-legend \
  --baseline-color '0.65' \
  --no-timing-note \
  --shade-migration-phase \
  --omit-incomplete-median-tail \
  --title '' \
  --x-label '' \
  --y-label '' \
  --no-y-tick-labels \
  --font-size 22 \
  --x-range 125 225 \
  --y-range 0 2250 \
  --x-tick-step 25 \
  --output /tmp/Main-Postcopy.pdf \
  --median-output logs_14_major/plots/Presentation/Main-Postcopy.pdf \
  --main-line-width 3.5 \
  --baseline-line-width 2.5 \
  --event-line-width 3.0

.venv/bin/python Scripts/plot_throughput.py \
  logs_14_major/Stop_Copy_4T \
  --plots throughput \
  --baseline-dir logs_14_major/Baseline_4T \
  --no-iqr \
  --compact-legend \
  --baseline-color '0.65' \
  --no-timing-note \
  --shade-migration-phase \
  --omit-incomplete-median-tail \
  --title '' \
  --x-label '' \
  --y-label '' \
  --no-y-tick-labels \
  --font-size 22 \
  --x-range 125 225 \
  --y-range 0 2250 \
  --x-tick-step 25 \
  --output /tmp/Main-Stop-and-copy.pdf \
  --median-output logs_14_major/plots/Presentation/Main-Stop-and-copy.pdf \
  --main-line-width 3.5 \
  --baseline-line-width 2.5 \
  --event-line-width 3.0

# Stress
.venv/bin/python Scripts/plot_throughput.py \
  logs_14_major/Precopy_Nonconvergent_16T \
  --plots throughput \
  --baseline-dir logs_14_major/Baseline_16T \
  --compact-legend \
  --baseline-color '0.65' \
  --no-iqr \
  --no-timing-note \
  --shade-migration-phase \
  --omit-incomplete-median-tail \
  --title '' \
  --x-label '' \
  --y-label '' \
  --font-size 22 \
  --x-range 75 212 \
  --y-range 0 4000 \
  --x-tick-step 25 \
  --output /tmp/Stress-Precopy.pdf \
  --median-output logs_14_major/plots/Presentation/Stress-Precopy.pdf \
  --main-line-width 3.5 \
  --baseline-line-width 2.5 \
  --event-line-width 3.0

.venv/bin/python Scripts/plot_throughput.py \
  logs_14_major/Postcopy_16T \
  --plots throughput \
  --baseline-dir logs_14_major/Baseline_16T \
  --no-iqr \
  --compact-legend \
  --baseline-color '0.65' \
  --no-timing-note \
  --shade-migration-phase \
  --omit-incomplete-median-tail \
  --title '' \
  --x-label '' \
  --y-label '' \
  --no-y-tick-labels \
  --font-size 22 \
  --x-range 75 212 \
  --y-range 0 4000 \
  --x-tick-step 25 \
  --output /tmp/Stress-Postcopy.pdf \
  --median-output logs_14_major/plots/Presentation/Stress-Postcopy.pdf \
  --main-line-width 3.5 \
  --baseline-line-width 2.5 \
  --event-line-width 3.0

# Hybrid
.venv/bin/python Scripts/plot_throughput.py \
  logs_14_major/Postcopy_Late_16T_25s \
  --plots throughput \
  --baseline-dir logs_14_major/Baseline_16T \
  --no-iqr \
  --compact-legend \
  --baseline-color '0.65' \
  --no-timing-note \
  --shade-migration-phase \
  --omit-incomplete-median-tail \
  --title '' \
  --x-label '' \
  --y-label '' \
  --font-size 22 \
  --x-range 75 175 \
  --y-range 0 4000 \
  --x-tick-step 25 \
  --output /tmp/Hybrid-Postcopy-25s.pdf \
  --median-output logs_14_major/plots/Presentation/Hybrid-Postcopy-25s.pdf \
  --main-line-width 3.5 \
  --baseline-line-width 2.5 \
  --event-line-width 3.0

.venv/bin/python Scripts/plot_throughput.py \
  logs_14_major/Autoconverge_16T \
  --plots throughput \
  --baseline-dir logs_14_major/Baseline_16T \
  --no-iqr \
  --compact-legend \
  --baseline-color '0.65' \
  --no-timing-note \
  --shade-migration-phase \
  --omit-incomplete-median-tail \
  --title '' \
  --x-label '' \
  --y-label '' \
  --no-y-tick-labels \
  --font-size 22 \
  --x-range 75 175 \
  --y-range 0 4000 \
  --x-tick-step 25 \
  --output /tmp/Hybrid-Autoconverge.pdf \
  --median-output logs_14_major/plots/Presentation/Hybrid-Autoconverge.pdf \
  --main-line-width 3.5 \
  --baseline-line-width 2.5 \
  --event-line-width 3.0

# El Restarto:
.venv/bin/python Scripts/plot_throughput.py \
  logs_14_major/Prewarmed_4T \
  --plots throughput \
  --restart-overlay-dir logs_14_major/Cold_Restart_4T \
  --primary-label Prewarmed \
  --restart-overlay-label Cold \
  --zero-restart-gap \
  --no-iqr \
  --compact-legend \
  --no-timing-note \
  --omit-incomplete-median-tail \
  --title '' \
  --x-label '' \
  --y-label '' \
  --font-size 22 \
  --x-range 0 300 \
  --y-range 0 2500 \
  --x-tick-step 25 \
  --output /tmp/Cold-vs-Prewarmed-throughput.pdf \
  --median-output logs_14_major/plots/Presentation/Cold-vs-Prewarmed-throughput.png \
  --main-line-width 3.5 \
  --event-line-width 3.0

.venv/bin/python Scripts/plot_throughput.py \
  logs_14_major/Prepared_4T \
  --plots throughput \
  --exclude-run 1 \
  --no-iqr \
  --compact-legend \
  --no-timing-note \
  --omit-incomplete-median-tail \
  --min-median-runs 8 \
  --title '' \
  --x-label '' \
  --y-label '' \
  --no-y-tick-labels \
  --shade-migration-phase \
  --font-size 22 \
  --x-range 0 300 \
  --y-range 0 2500 \
  --x-tick-step 25 \
  --output /tmp/Prepared-throughput.pdf \
  --median-output logs_14_major/plots/Presentation/Prepared-throughput.png \
  --main-line-width 3.5 \
  --event-line-width 3.0