# Lesson 1
- `pd.read_csv(low_memory=False, parse_dates)` https://youtu.be/CzdWqFTmn0Y?t=1717
- display_all function for df: https://youtu.be/CzdWqFTmn0Y?t=1929
- log error cares about ratio rather than value: https://youtu.be/CzdWqFTmn0Y?t=2107
- add_datepart: https://youtu.be/CzdWqFTmn0Y?t=3072
- train_cat/apply_cat: https://youtu.be/CzdWqFTmn0Y?t=3467
- `.dt` and `.cat` and `.cat.set_categories(ordered=True)`: https://youtu.be/CzdWqFTmn0Y?t=3595
- make a tmp dir: https://youtu.be/CzdWqFTmn0Y?t=3988
- `to_feather`: https://youtu.be/CzdWqFTmn0Y?t=3931
- `proc_df`: https://youtu.be/CzdWqFTmn0Y?t=4087
- `fix_missing`: https://youtu.be/CzdWqFTmn0Y?t=4167
- `df.items()`: https://youtu.be/CzdWqFTmn0Y?t=4246
- including IDs works fine: https://youtu.be/CzdWqFTmn0Y?t=4330
- RandomForrest `n_jobs=-1`: https://youtu.be/CzdWqFTmn0Y?t=4345
- `print_score`: https://youtu.be/CzdWqFTmn0Y?t=4483

# Lesson 2
- link source code `ln -s`: https://youtu.be/blyXCk4sgEg?t=149
- pandas categories: https://youtu.be/blyXCk4sgEg?t=529
- r-squared explained: https://youtu.be/blyXCk4sgEg?t=758
- `proc_df(subset=)`: https://youtu.be/blyXCk4sgEg?t=1844
- RandomForrest `boostrap=False` and `draw_tree`: https://youtu.be/blyXCk4sgEg?t=1935
- Bagging of little bootstraps: https://youtu.be/blyXCk4sgEg?t=2858
- Less predictive and less correlated trees: https://youtu.be/blyXCk4sgEg?t=3442
- each tree can predict in RF: https://youtu.be/blyXCk4sgEg?t=3879
- 20-30 trees, 1000 trees over night: https://youtu.be/blyXCk4sgEg?t=4143
- RF out of bag validation `oob_score`: https://youtu.be/blyXCk4sgEg?t=4225
- `set_rf_samples`: https://youtu.be/blyXCk4sgEg?t=4600
- `min_samples_leaf`: https://youtu.be/blyXCk4sgEg?t=4953
- `max_features`: https://youtu.be/blyXCk4sgEg?t=5054
- RF never remove variables after each split: https://youtu.be/blyXCk4sgEg?t=5238
- Order of categorical variables (not one-hot) doesn't matter: https://youtu.be/blyXCk4sgEg?t=5577

# Lesson 3
## Kaggle Grocery
- set `dtype` in `read_csv` for large files : https://youtu.be/YSFG_W8JxBo?t=964
- SIMD: https://youtu.be/YSFG_W8JxBo?t=1192
- `shuf` read in a random sample of large csv: https://youtu.be/YSFG_W8JxBo?t=1243
- `describe(include='all')`: https://youtu.be/YSFG_W8JxBo?t=1371
- how long RF runs depends on what: https://youtu.be/YSFG_W8JxBo?t=1784
- `prun`, profiler: https://youtu.be/YSFG_W8JxBo?t=1862
- validation score v.s. kaggle score correlation - how to check val set is good: https://youtu.be/YSFG_W8JxBo?t=2694
## Interpreting ML models
- confidence of prediction - standard deviation of the predictions of trees: https://youtu.be/YSFG_W8JxBo?t=3402
- `parallel_tree`: https://youtu.be/YSFG_W8JxBo?t=3633
- pandas plotting: 
  - https://youtu.be/YSFG_W8JxBo?t=3768
  - https://youtu.be/YSFG_W8JxBo?t=3887
- pandas `groupby(as_index=False)`: https://youtu.be/YSFG_W8JxBo?t=3855
- feature importance: https://youtu.be/YSFG_W8JxBo?t=4051
- trust this feature importance better: https://youtu.be/YSFG_W8JxBo?t=4630
- how to get feature importance: https://youtu.be/YSFG_W8JxBo?t=4679

# Lesson 4
- RF hyperparameters: 
  - https://youtu.be/0v93qHDqq_g?t=144
  - Values for parameters to try: https://youtu.be/0v93qHDqq_g?t=1096
- Use oob to check overfitting: https://youtu.be/0v93qHDqq_g?t=2029
- issues with traditional feature importance: https://youtu.be/0v93qHDqq_g?t=2249
- one-hot 
  - https://youtu.be/0v93qHDqq_g?t=2467
  - for RF, not mendatory


