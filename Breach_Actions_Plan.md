# Breach Action Steps

This is a 4-step plan as to how to react when there has been a data breach (patient identifiable information, trust sensitive information, API keys, etc).

## STEP 1: Take a copy
The documentation recommends taking a copy of the repository before making any changes. The code on the BFG Repo-Cleaner is for the Terminal or you can copy local folders.

## STEP 2:  Clean
GitHub recommend using [BFG Repo-Cleaner](https://rtyley.github.io/bfg-repo-cleaner/) for a quick and efficient way of deleting files, their history from the commit and this can be used across all branches.
BFG Repo-Cleaner is also good for removing very large files.

It requires [Java](https://www.java.com/en/download/manual.jsp) installed and this may also require administrator rights to do as well as the [BFG Repo-Cleaner `.jar` file](https://repo1.maven.org/maven2/com/madgag/bfg/1.14.0/bfg-1.14.0.jar).

Once downloaded put the `bfg-1.14.0.jar` in the folder where the file is that you wish to delete.

Delete the file and commit that so that the latest commit is _clean_ and doesn't contain the undesired data.

Using the Terminal type (on Windows)

```
java -jar bfg-1.14.0.jar -–delete-files my_sensitive_file.rda

```
If the file and `bfg-1.14.0.jar` are in a subfolder amend the code for the `bfg-1.14.0.jar` part only:

```
java -jar example\subfolder\bfg-1.14.0.jar -–delete-files my_sensitive_file.rda

```

If it works then you should get a whole list of information about the deletion.
However, if it doesn't work then you will get information on the ways you can use the program.

If the sensitive data is part of something like a Quarto report, website or book then a corresponding `html` file will also have to be deleted. Once the file history has been removed from the Git history type:

```
git push --force

```
## STEP 3:  Contact GitHub

Using the BFG Repo-Cleaner changes the Git history on main and may also do this for branches.

Anything that has already been cloned, forked or downloaded from GitHub will be unaffected and you may need to contact GitHub directly to ensure this information is removed from GitHub repositories.


## STEP 4:  Raise incident

Any publishing of sensitive data will require an incident to be raised within your organisation and may be classed as a breach and this can cause stress and pressure in the people involved. In order to react quickly and efficiently it's advisable to practice deleting Git histories that don't involve sensitive information.



