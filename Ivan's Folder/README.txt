Greybox Modeling Of The Heat Evolution Of CO2 Capture In Amine-Based Liquid Solvents

The project is divided into two main parts: the Analytical Model and the CTSM Model.



The Analytical Model folder contains:
- Analytical Model.ipynb: the code for the analytical model
- csv/ : contains the training data in CSV format, with each file representing a different region or time period.

- T_no_heat.pdf: estimation of effective thermal diffusivity based on data without heat production.
- Temperature profile (2 ODEs, interface at point 1.5).pdf: 17 fits obtained from the analytical model.
- Training Data Plots/ : contains training data plots.



The CTSM Model folder contains:
- final_ctsm.Rmd: the code for the CTSM model.
- csv/ : contains the training data in CSV format, with each file representing a different region or time period.

- dynamic_mu/ : dynamic mu model trained on "March 3" data, including data, fits, residual analysis, and parameter estimates in R output files.
- fixed_mu/ :   fixed mu model trained on "June short" data, including data, fits, residual analysis, and parameter estimates in R output files.

- Other CTSM Models For Comparison: contains other 5 CTSM models: 
    - dynamic_mu_no_k4_sigma_x4:            a dynamic mu model without k4 and sigma_x4 parameters, trained on "March 3" data.
    - dynamic_mu_no_P_loss:                 a dynamic mu model without P_loss, trained on "March 3" data.
    - dynamic_mu_no_k4_sigma_x4_P_loss:     a dynamic mu model without k4, sigma_x4, and P_loss parameters, trained on "March 3" data.
    - dynamic_mu_yT1:                       a dynamic mu model with yT1 parameter, trained on "March 3" data.
    - fixed_mu_yT1:                         a fixed mu model with yT1 parameter, trained on "June short" data.

- dynamic_mu model comparison.txt: a comparison of the dynamic mu model with other dynamic models trained on "March 3" data.
- fixed_mu model comparison.txt: a comparison of the fixed_mu model with other models trained on "June short" data.




Folder Structure:
.
├── Analytical Model
│   ├── Analytical Model.ipynb
│   ├── csv
│   │   ├── df complete 1.csv
│   │   ├── df complete 10.csv
│   │   ├── df complete 11.csv
│   │   ├── df complete 12.csv
│   │   ├── df complete 13.csv
│   │   ├── df complete 14.csv
│   │   ├── df complete 15.csv
│   │   ├── df complete 16.csv
│   │   ├── df complete 17.csv
│   │   ├── df complete 2.csv
│   │   ├── df complete 3.csv
│   │   ├── df complete 4.csv
│   │   ├── df complete 5.csv
│   │   ├── df complete 6.csv
│   │   ├── df complete 7.csv
│   │   ├── df complete 8.csv
│   │   └── df complete 9.csv
│   ├── T_no_heat.pdf
│   ├── T_no_heat.svg
│   ├── Temperature profile (2 ODEs, interface at point 1.5).pdf
│   └── Training Data Plots
│       ├── 2024_June_region_10.png
│       ├── 2024_June_region_8.png
│       ├── 2024_June_region_9.png
│       ├── 2024_June.png
│       ├── 2024_May_region_1.png
│       ├── 2024_May_region_2.png
│       ├── 2024_May_region_3.png
│       ├── 2024_May_region_4.png
│       ├── 2024_May_region_5.png
│       ├── 2024_May_region_6.png
│       ├── 2024_May_region_7.png
│       ├── 2024_May.png
│       ├── 2025_March_region_11.png
│       ├── 2025_March_region_12.png
│       ├── 2025_March_region_13.png
│       ├── 2025_March_region_14.png
│       ├── 2025_March_region_15.png
│       ├── 2025_March_region_16.png
│       ├── 2025_March_region_17.png
│       └── 2025_March.png
├── CTSM Model
│   ├── csv
│   │   ├── 2024_June.csv
│   │   ├── 2024_May.csv
│   │   └── 2025_March.csv
│   ├── dynamic mu model comparison.txt
│   ├── dynamic_mu
│   │   ├── ctsm dynamic_mu model.txt
│   │   ├── dynamic_mu March 3 data.png
│   │   ├── dynamic_mu March 3 fit.png
│   │   ├── dynamic_mu March 3 Routput.txt
│   │   ├── dynamic_mu March 3 T2.png
│   │   ├── dynamic_mu March 3 T3.png
│   │   └── dynamic_mu March 3 T4.png
│   ├── final_ctsm.Rmd
│   ├── fixed mu model comparison.txt
│   ├── fixed_mu
│   │   ├── ctsm fixed_mu model.txt
│   │   ├── fixed_mu June short data.png
│   │   ├── fixed_mu June short fit.png
│   │   ├── fixed_mu June short Routput.txt
│   │   ├── fixed_mu June short T2.png
│   │   ├── fixed_mu June short T3.png
│   │   └── fixed_mu June short T4.png
│   └── Other CTSM Models For Comparison
│       ├── dynamic_mu_no_k4_sigma_x4 March 3 data.png
│       ├── dynamic_mu_no_k4_sigma_x4 March 3 fit.png
│       ├── dynamic_mu_no_k4_sigma_x4 March 3 Routput.txt
│       ├── dynamic_mu_no_k4_sigma_x4 March 3 T2.png
│       ├── dynamic_mu_no_k4_sigma_x4 March 3 T3.png
│       ├── dynamic_mu_no_k4_sigma_x4 March 3 T4.png
│       ├── dynamic_mu_no_k4_sigma_x4_P_loss March 3 data.png
│       ├── dynamic_mu_no_k4_sigma_x4_P_loss March 3 fit.png
│       ├── dynamic_mu_no_k4_sigma_x4_P_loss March 3 Routput.txt
│       ├── dynamic_mu_no_k4_sigma_x4_P_loss March 3 T2.png
│       ├── dynamic_mu_no_k4_sigma_x4_P_loss March 3 T3.png
│       ├── dynamic_mu_no_k4_sigma_x4_P_loss March 3 T4.png
│       ├── dynamic_mu_no_P_loss March 3 data.png
│       ├── dynamic_mu_no_P_loss March 3 fit.png
│       ├── dynamic_mu_no_P_loss March 3 Routput.txt
│       ├── dynamic_mu_no_P_loss March 3 T2.png
│       ├── dynamic_mu_no_P_loss March 3 T3.png
│       ├── dynamic_mu_no_P_loss March 3 T4.png
│       ├── dynamic_mu_yT1 March 3 data.png
│       ├── dynamic_mu_yT1 March 3 fit.png
│       ├── dynamic_mu_yT1 March 3 Routput.txt
│       ├── dynamic_mu_yT1 March 3 T2.png
│       ├── dynamic_mu_yT1 March 3 T3.png
│       ├── dynamic_mu_yT1 March 3 T4.png
│       ├── fixed_mu_yT1 June short data.png
│       ├── fixed_mu_yT1 June short fit.png
│       ├── fixed_mu_yT1 June short Routput.txt
│       ├── fixed_mu_yT1 June short T2.png
│       ├── fixed_mu_yT1 June short T3.png
│       └── fixed_mu_yT1 June short T4.png
├── README.txt
└── settings.json

9 directories, 93 files