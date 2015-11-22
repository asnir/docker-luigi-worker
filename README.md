Example for [Luigi](http://luigi.readthedocs.org/en/latest/index.html) worker

 Reminder: Task pool doesn't exist at this paradigm. The worker execute all the steps at the workflow (Distrubation of work is not supported). 
 For more info please review [design & limitations](http://luigi.readthedocs.org/en/stable/design_and_limitations.html)
 
 Each worker will execute specific workflow.

```bash
#Building the image
docker build -t luigi_worker .

#Lifting up container.
docker run -it --rm --name luigi_worker1 luigi_worker
```
