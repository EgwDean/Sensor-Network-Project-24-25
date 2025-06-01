# AIoT Course - Human Gesture Recognition Project

## Deliverables' Structure:

```
deliverables/
├── README.md
├── requirements.txt
├── utils_visual.py
├── utils.py
├── config.yml
├── aiot_project.ipynb
├── aiot_dataset_creation.ipynb
└── data/
    ├── class_A/
    │   ├── data_A_01.csv
    │   ├── data_A_02.csv
    │   ├── data_A_03.csv
    │   ├── data_A_04.csv
    │   └── data_A_05.csv
    ├── class_D/
    │   ├── data_D_01.csv
    │   ├── data_D_02.csv
    │   ├── data_D_03.csv
    │   ├── data_D_04.csv
    │   └── data_D_05.csv
    ├── class_L/
    │   ├── data_L_01.csv
    │   ├── data_L_02.csv
    │   ├── data_L_03.csv
    │   ├── data_L_04.csv
    │   └── data_L_05.csv
    ├── class_M/
    │   ├── data_M_01.csv
    │   ├── data_M_02.csv
    │   ├── data_M_03.csv
    │   ├── data_M_04.csv
    │   └── data_M_05.csv
    └── class_U/
        ├── data_U_01.csv
        ├── data_U_02.csv
        ├── data_U_03.csv
        ├── data_U_04.csv
        └── data_U_05.csv
```

## Requirements:
- The requirements can be found at the ``requirements.txt`` file. The libraries installed are the same as the ones in the original file with the addition of one more. It is used to plot the architecture of the CNN used. It can be either installed using ``pip install -r requirements.txt`` or ``pip install graphviz==0.20.3``. It requires [Graphviz](https://graphviz.gitlab.io/download/) to be installed. The version the project used was **graphiz 12.2.1**. Make sure to add it to path.

- A **MongoDB** service needs to be active.

## Execution:
- ``utils.py`` and ``utils_visual.py`` were not changed.
- ``config.yml`` includes the parameters of the models used.
- ``aiot_dataset_creation.ipynb`` initializes the database and should be run first.
- ``aiot_project.ipynb`` contains the rest of the project
- The whole project can be run sequencially, by running the code in the cells found the two above files.

## Gestures' Collection:
The watch data were collected in the following way:

- The watch was worn on the right hand of the person who performed the movements.  
- All movements for the letters were performed while sitting down on a chair, in the exact same position.  
- For each of the five letters: A, D, L, M, and U, there are five measurements. The duration of each measurement is exactly ten seconds long, meaning that there are fifty seconds of data for each letter.  
- For all measurements, the movement of the right hand began before starting the measurement and concluded after the measurement was completed.