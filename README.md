# Motion-based post-processing: Using Kalman Filter to Exclude Similar Targets in Underwater Object Tracking

## Our method
Our code will be released after the manuscript is received

## Evaluation
Raw results can be found here [[Baidu Drive](https://pan.baidu.com/s/1Z45Op05GVSiGvACfYB9FCw?pwd=0000)] (password: 0000) [[Google Drive]](https://drive.google.com/drive/folders/1FKIV6jBGdz6nK6BaFRDSLvMjtvZ_F_Ax?usp=share_link)

Download UOT100(https://www.kaggle.com/datasets/landrykezebou/uot100-underwater-object-tracking-dataset)

Download UTB180(https://www.kaggle.com/datasets/bastech/utb180)

Put UOT100 and UTB in ./data. It should look like:

   ```
   ${PROJECT_ROOT}
    -- data
        -- UOT100
            |-- AntiguaTurtle
            |-- ArmyDiver1
            |-- ArmyDiver2
            ...
        -- UTB180
            |-- Video_0001
            |-- Video_01
            |-- Video_0002
            ...
   ```
Merge the provided code with original [[OSTrack](https://github.com/botaoye/OSTrack)] framework

Go to `lib/test/evaluation/local.py` to set datasets dir

Then you can test your tracker in UOT100 and UTB180 or evaluate our raw results


- UOT100

Put the UOT100 raw results  on `$PROJECT_ROOT$/output/test/tracking_results/`
```
python tracking/analysis_results.py # need to modify tracker configs and names
```
- UTB180

Put the UTB180 raw results  on `$PROJECT_ROOT$/output/test/tracking_results/`

```
python tracking/analysis_results.py # need to modify tracker configs and names
```


## Acknowledgments
* Thanks for the [OStrack](https://github.com/botaoye/OSTrack) library, which helps us to quickly implement our ideas.
