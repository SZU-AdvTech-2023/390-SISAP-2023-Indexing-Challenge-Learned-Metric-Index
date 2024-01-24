```bash
conda create -n env python=3.8
conda activate env
conda install matplotlib pandas scikit-learn
pip install h5py flake8 setuptools tqdm faiss-cpu
pip install torch --index-url https://download.pytorch.org/whl/cpu
```

### Running
```bash
pip install --editable .
python search/search.py # for 10M index
python search/search.py --size=300K -bp 6 # for 300K index
```

### Evaluation
```bash
python eval/eval.py
python eval/plot.py res.csv
cat res.csv
```
