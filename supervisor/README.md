# bash
A Daemon Supervisor which should check that the process is running and at all times and starts it in case is down. 
Parameters that it should take:
	+ Seconds to wait between attempts to restart service
	+ Number of attempts before giving up
	+ Name of the process to supervise
	+ Check interval in seconds
	+ Generate logs in case of events.