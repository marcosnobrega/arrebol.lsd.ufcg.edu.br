Title: Running a Job
url: running-a-job
save_as: running-a-job.html
section: runningajob
index: 2

Running a Job
==========

How to run a Job

------

After unpacking a Arrebol release package (listed here), the Arrebol CLI script can be found in bin/directory.
To submit a JDF-formatted job, run the arrebol script with the POST command:
job_id=`bin/arrebol.sh POST jdf_file_path optionals: -f [friendly name] -s [schedule path]`
It is mandatory to specify the path of the JDF-formatted file which describes the job. There are also two optional arguments: the job friendly name (specified with the -f flag) and the schedule path (specified with the -s flag). The friendly name gives a human-readable name. The scheduler path indicates to the Submission service a file system path where it can find the data processed by a submitted job. On sucessful execution, the bin/arrebol.sh script outputs a unique identifier to the submitted job.
To retrieve status information about all running jobs, run the arrebol script with the GET command:
bash bin/arrebol.sh GET
To retrieve information about a specific running job, run the arrebol script witht GET and specify the job id or the the job friendly name.
bash bin/arrebol.sh GET [job id or friendly name]
To stop a running job, run the arrebol script with the STOP command with the associated job id or friendly name.
bash arrebol.sh STOP [job id or friendly name]




