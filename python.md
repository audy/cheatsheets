# pip

- `-e git://github.com/mozilla/elasticutils.git#egg=elasticutils` - specify a
  Git repository in a `requirements.txt` file.

# jupyter

- `%config InlineBackend.figure_format = 'retina'` - 2x resolution plots for
  retina display.
- `%load_ext autoreload; %autoreload 2` - reload imports automatically.
- `pylab.rcParams['figure.figsize'] = (10, 6)` - larger plots.

# pandas

Group DataFrame and take top row

```python
best = dat.\
          groupby('column1').\
          agg(lambda x: x.loc[x['column2'].argmax(),])
```
