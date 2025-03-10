## Figure 6

### :white_check_mark: Pre-requisites
The code scripts in this directory requires the CSV satisficing files in `scripts/Phase2/output` and the Pathways `.out` files in the `scripts/Phase2/output/solXX__objs_pathways/` folder. Please navigate to the [Phase 2 page](https://github.com/lbl59/TRAILS/tree/main/scripts/Phase2) to complete all the steps listed there before attempting this section.

### :computer: Generating the figure
To generate Figures 6(a and b), (c and d) separately, run the code in the order shown in the table below. The figures can then be combined using a figure editor like Adobe Illustrator.

| Figure| Script Name | Description | How to Run | Pre-requisite files | 
| --- | --- | --- | --- | --- |
| NA | `custom_colormap.py` | Contains the function that enables a custom colormap to be plotted in `plot_infra_counts_baseline.py`. | None | None |
| 6(a and b) | `plot_robustness_timeseries.py` | Plots the robustness timeseries for each utility and the region as a whole. | `python ./calc_plot_robustness_change.py` | The satisficing CSV files in `scripts/Phase2/output/` |
| 6(c and d) | `plot_infra_counts_baseline.py` | Plots the infrastructure bar and KDE likelihood plots. | `python ./plot_infra_counts_baseline.py` | The `.out` files in the `scripts/Phase2/output/solXX__objs_pathways/` for Solution XX |

The `plot_infra_counts_baseline.py` script also plots `FigureSI_infraDF.jpg` and `FigureSI_infraRR.jpg` in the `figures/supporting/` folder found [here](https://github.com/lbl59/TRAILS/tree/main/figures/supporting).

### :pushpin: Figure generation outputs
If `plot_robustness_timeseries.py` was run correctly, you should see a new `critical_periods/` folder created in your current directory. This folder should contain 2-column CSV files that contain your start and ending weeks of the robustness conflict periods for the region. This will come in handy when generating Figures 7, 8, and 9.

[Back to main README](https://github.com/lbl59/TRAILS)