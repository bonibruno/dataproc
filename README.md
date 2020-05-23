Dataproc is Google's Cloud Managed Hadoop/Spark Service.  You can use cloud shell commands to quickly create a hadoop cluster.  

I provide the cloud shell commands to create a Dataproc Hadoop Cluster and to also launch TeraGen, TeraSort, and TeraValidate jobs.  These jobs are good for benchmarking your cluster.

Replace project-name with your Google Cloud project and bucket-name with your Google Storage Bucket Name.  You need a storage bucket to store data, if you already have a Google Storage Bucket, skip the gsutil command.

Note:  The default quota is 2400 CPUs, so if you need a cluster that is larger than 2400 CPUs, send a request to Google to increase your quota limit.  

If this is for testing pruposes, don't forget to delete your cluster when your done with:
gcloud dataproc clusters delete (cluster-name).

I also created an HDP 3.1 cluster on the same number and type of instances used for dataproc, but intead of using Google's object storage I used Dell Technologies Cloud OneFS HDFS storage and stored the results in the attached spreadsheet.  It was impressive to see that Cloud OneFS outperform Google Cloud Storage which is massive.  Furthermore, The Cloud OneFS system tested only had 56 nodes and only half the number of network connections were enabled at the time of testing.  

Regards,

boni bruno

