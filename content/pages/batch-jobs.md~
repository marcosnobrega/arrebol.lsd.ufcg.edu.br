Title: Batch Jobs
url: batch-jobs
save_as: batch-jobs.html
section: batchjobs
index: 4

Batch Jobs
==========

Creating and running batch Jobs

------

Batch jobs is a way to generate big repetitive jobs in a quick way, to make use to it to have to create two files:
The blueprint file specifies the placeholders:
        put $1 /tmp/$1
        python mysimulation.py < /tmp/$1 > /tmp/$2
        get /tmp/$2 $2


it is the basic structure of each task you wish to run
The parameter sweep file defines values to replace the placeholders:
        simulationentries1 outputfile1
        simulationentries2 outputfile2


The generated file will look like this:
        job:
        task:
        put simulationentries1 /tmp/simulationentries1
        python mysimulation.py  /tmp/simulationentries1 > /tmp/outputfile1
        get /tmp/outputfile1 outputfile1
        task:
        put simulationentries2 /tmp/simulationentries2
        python mysimulation.py  /tmp/simulationentries2 > /tmp/outputfile2
        get /tmp/outputfile2 outputfile2


After that just run:
        python bin/batch_arrebol jdf_blueprint_path param_sweep_pat > jobfilename.jdf
Then run the resulting file as usual




