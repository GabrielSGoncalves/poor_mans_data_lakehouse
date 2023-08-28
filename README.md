# Poor Man's Data Lakehouse

## Environment setup
```bash
poetry new poor_mans_data_lakehouse
```

```bash
poetry add pandas polars duckdb deltalake jupyterlab ipykernel boto3 kaggle
```

```bash
poetry run ipython kernel install --user --name=poor-mans-datalakehouse
```

```bash
mkdir datasets 
cd datasets
poetry run kaggle datasets download -d jeffsinsel/nyc-fhvhv-data
kaggle datasets download -d netflix-inc/netflix-prize-data
unzip kensho-derived-wikimedia-data.zip
```




```bash
poetry run jupyter lab
```


## References
https://dataschool.com/data-modeling-101/running-jupyter-notebook-on-an-ec2-server/
https://delta-io.github.io/delta-rs/python/
https://www.kaggle.com/datasets/jeffsinsel/nyc-fhvhv-data
https://www.mage.ai/blog/how-to-build-a-data-pipeline-using-delta-lake
https://www.databricks.com/blog/2020/08/21/top-5-reasons-to-convert-your-cloud-data-lake-to-a-delta-lake.html