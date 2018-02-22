Hello! In this microtask, we will try to list out all the new committers that commit to a repository each month and the number of commits that they do.

We will list out their names and the number of commits in a table using pandas and then we will store it in a csv file.
This is essentially what Microtask-1 is.

The analysis is in the Jupyter-Notebook.

---

We will start with choosing a repository to analyse. I am analysing [aima-python](https://github.com/aimacode/aima-python.git)

If you followed the instructions in the README.md at the home page then you have the necessary libraries and Elasticsearch installed. 

We'll have to index and enrich the data in the repository. For that we should run the command:
```
p2o.py --enrich --index <raw index name> --index-enrich <enriched index name> \
  -e http://localhost:9200 --no_inc --debug \
  git <URL of the repository to analyse>
```

For me the command will be:
```
p2o.py --enrich --index aima_python_raw --index-enrich aima_python \
  -e http://localhost:9200 --no_inc --debug \
  git https://github.com/aimacode/aima-python.git
```
**HERE: `localhost:9200` is the address of the Elasticsearch server**

More instructions on how to enrich and upload an index to elasticsearch [here](https://grimoirelab.gitbooks.io/tutorial/grimoireelk/a-simple-dashboard.html).

Now start the Jupyter server and head over to the notebook for the analysis part. You can learn about Jupyter Notebooks [here](http://jupyter.org/).