# dropzflow
workflow scripts for dropz

* [ ] open up console in that directory and run ``./scenario`` to install 
* [ ] change directory to dropz root.
* [ ] try ``scenario 855 company-admatees/investors``
* [ ] wipe that tear from your cheek

but… but what does it do?
* first off, it adds its path to fish's PATH var ("what I call setup :D")
* on next run it parses the issue's content for the first occurence of **" #666"** to know what the **parent issue** is
* it then creates a **feature branch** for it
* **switches** to that branch
* creates the **folder structure** in cucumber/tests if necessary
* creates the **feature file** (if necessary) and fills it with the first **````gherkin** block from the *parent issue*
* **adds the scenario** from the current issue to the feature file
* creates the **step definition file** (if necessary) and fills it with the implementations including regExp
* adds the changes to GIT and creates a new commit