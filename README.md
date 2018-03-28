This repository contains the Microtasks for the project: Reporting CHAOSS mertics. Details [here](https://github.com/chaoss/grimoirelab/issues/70).

---

[X] **Microtask 1**: Produce a listing of the number of new committers per month, and the number of commits for each of them, as a table and as a CSV file. Use the GrimoireLab enriched index for git. The CSV file can be found [here](Microtask-1/aima_python_git.csv)

[X] **Microtask 2**: Produce a chart showing the distribution of time-to-close (using the corresponding field in the GrimoireLab enriched index for GitHub issues) for issues already closed, and opened during the last six months.
![time to close](https://github.com/aswanipranjal/chaoss-microtasks/blob/master/Images/time_to_close.png)

[X] **Microtask 3**: Produce a listing of repositories, as a table and as CSV file, with the number of commits authored, issues opened, and pull requests opened, during the last three months, ordered by the total number (commits plus issues plus pull requests). The CSV file can be found [here](Microtask-3/Indices.csv)

**Microtask 4**: Perform any other analysis you may find interesting, based on GrimoireLab enriched indexes for git and GitHub repositories.

---
*Optional*

[X] **Microtask 5**: Produce a pull request for any of the GrimoireLab tools, and try to follow instructions until it gets accepted. Try do do something simple that you consider useful, not necessarily fix to the code: improvement of comments, documentation or testing will usually be easier to get accepted, and very useful for the project. Please, avoid just producing a random pull request just to have another microtask: the objective is not that you get one more microtask done, but that you understand how to interact with developers in the project contributing with something that could be useful).

For this microtask, I produced 2 pull requests:
- The First one was to add a `Content-Type` header to the request that was being made to the Elasticsearch instance. This PR makes Manuscripts compatible with Elasticsearch-6. You can find it [here](https://github.com/chaoss/grimoirelab-manuscripts/pull/18).

- The Second PR changed the default name of the git enriched index from `git_enrich` to `git`. And it added the functionality for the user to be able to provide custom index names for the elasticsearch indices that they use while creating the reports. You can find it [here](https://github.com/chaoss/grimoirelab-manuscripts/pull/26).

---
### To do these analysis your self, follow these instructions:

1. Clone the repository:
```
git clone https://github.com/aswanipranjal/chaoss-microtasks.git
```

2. Download Elasticsearch [**Optional:** Download *Kibana* if you want to visualise all the data in beautiful charts and bar graphs]

3. Download necessary libraries and go through the [Grimoire Turorial](https://www.gitbook.com/book/grimoirelab/tutorial)

---

Each folder contains one microtask. Start with reading the corresponding Microtask-x.md file to learn more about it.
