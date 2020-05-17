Dataproc is Google's Cloud Managed Hadoop/Spark Service.  You can use cloud shell commands to quickly create a hadoop cluster.  

I provide the cloud shell commands to create a Dataproc Hadoop Cluster and to also launch TeraGen, TeraSort, and TeraValidate jobs.  These jobs are good for benchmarking your cluster.

Replace project-name with your Google Cloud project and bucket-name with your Google Storage Bucket Name.  You need a storage bucket to store data, if you already have a Google Storage Bucket, skip the gsutil command.

Note:  The default quota is 2400 CPUs, so if need a cluster that is larger than 2400 CPUs, send a request to Google to increase your quota limit.  

Regards,

boni bruno
