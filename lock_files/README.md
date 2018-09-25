This code creates a .lock file upon commencing the kjb. When the job is complete, the .lock is deleted. If the ETL were to fail, the next
iteration of the job would immediately fail because the .lock file still exists from the previous run. This would prompt the administrator
to check why the previous execution failed before executing a new instance of the ETL.
