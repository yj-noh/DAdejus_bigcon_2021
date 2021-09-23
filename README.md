# Big Contest Championship league 
> Team `Da dejus`
> [@`lhmlhm1111`](https://github.com/lhmlhm1111) [@`codenavy94`](https://github.com/codenavy94) [@`dockjong`](https://github.com/dockjong) [@`Hail-cali`](https://github.com/Hail-cali)
## Baseball ops prediction

### Code description
- **how to train?** 
    -  we worked code based on shell command with python for faster hyper parameter tuning
    - the major options you should input, are `-models` `--y_feature`, `--file`, `--data_path`
    - for `-models`, `-l` option is model list you want to train, it is mapped inside code with dict
  
```shell
python final_train.py -l xgb lgbm rf --data_path  ./dataset --file train.csv --y_feature 장타
```

- **hyper parameter tuning** 
```shell
python run_grid.py -l xgb lgbm rf --data_path  ./dataset --file train.csv --y_feature 장타
```
- **gird_search & inference** 
```shell
python run_grid_stack.py -l xgb lgbm rf --data_path  ./dataset --file train.csv --y_feature 출루
```
<hr/>

### serving dataset

- the major option for making dataset from raw is `ws` (windeow size) and
 `agg`(aggregation rule |date | game|)
  

### modeling
- we used stacking ensemble model


