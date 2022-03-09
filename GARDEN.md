gantt
    title Garden 2022
    dateFormat  YYYY-MM-DD
    axisFormat  %b

    section Weather
    %% 2022            : t1, 2022-01-01, 365d
    Spring Thaw     : milestone, thaw, 2022-05-21, 1d
    Outdoor Growing Season  : og1, 2022-05-21, 2022-09-15
    Fall Freeze     : milestone, freeze, 2022-09-15, 1d

    %% section Onion (Candy Hybrid, Gurney's)
    %% Germinate   : o1, after thaw, 12d
    %% Plant       : milestone, after thaw
    %% Mature      : 02, after thaw, 85d
    
    section Jalapeno (Primo 2 Hybrid, Gurney's)
    Germinate   : j1, 2022-04-01 , 20d
    Plant       : milestone, after j1
    Mature      : j2, after j1, 75d

    section Dill (Mammoth, Gurney's)
    Germinate   : j1, 2022-04-01 , 14d
    Plant       : milestone, after j1
    Mature      : j2, after j1, 60d
