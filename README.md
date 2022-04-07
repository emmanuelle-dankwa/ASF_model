# ASF_model

## About 

The scripts and data held in this repository reproduces the results of the African swine fever (ASF) model as presented in the manuscript:

Dankwa, E.A, Lambert, S., Hayes, S., Thompson, R.N., Donnelly, C.A. Stochastic spatiotemporal of African swine fever in wild boar and domestic pigs: epidemic forecasting and comparison of disease management strategies. 


## Contents

The repository contains three folders and three data documentation files.

The folders are:

* `pig_herd_component`: contains files for modelling ASF infection dynamics in pig herds  
     
     Subfolders are:    
  + `Phase1`: files for Phase 1 model; refer to `documentation_phase1_ph.pdf` for details 
  + `Phase2`: files for Phase 2 model; refer to `documentation_phase2_ph.pdf` for details     
  + `Phase3`: files for Phase 3 model; refer to `documentation_phase3_ph.pdf` for details
       
* `wild_boar_component`: contains files for modelling ASF infection dynamics in wild boar
   
     Subfolders are:  
  + Phase 1: files for Phase 1 model; refer to `documentation_phase1_wb.pdf` for details 
  + Phase 2: files for Phase 2 model; refer to `documentation_phase2_wb.pdf` for details 
  + Phase 3: files for Phase 3 model; refer to `documentation_phase3_wb.pdf` for details
        
* `time_series_plots_all`: contains files for producing incidence plots of model predictions under the disease management measures and sensitivity analysis scenarios considered 
      
     Subfolders are:
  + `scripts`: contains the files
      - `organize_data_for_plots.R`, for organizing data for plots; and
      - `time_series_plots_script.R`, for producing plots given plotting data
  + `data`: contains `plotting_data_scenarios.rda`, which holds all data for incidence plots


The documentation files are `Phase 1 model data documentation.pdf`, `Phase 2 model data documentation.pdf` and `Phase 3 model data documentation.pdf`, for model input and output data at Phase 1, Phase 2 and Phase 3, respectively. These files are referenced in the phase-specific documentation in `pig_herd_component` and  `wild_boar_component`.  



## Reproduce results 

The setup of the repository allows the pig herd and wild boar components of the model to be analyzed separately, and independently for each phase. 

To reproduce results for wild boar herds at any phase, 
 + navigate to the desired phase folder 
 + run `master_script_....R` in the `scripts` folder.
       
To reproduce results for pig herds at any phase,
 + navigate to the desired phase folder
 + run `ASF_model.R` in the `Model_Predict` folder.

## Queries

Queries and suggestions are always welcome. Please email Emmanuelle at dankwa@stats.ox.ac.uk with such. 

## License

MIT License     
