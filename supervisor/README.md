# Daemon Supervisor


A Daemon Supervisor which should check that the process is running and at all times and starts it in case is down. 

## Directories

  - `config`: include config.json which contains variables such as
  
        - `SERVICE_NAME`: Name of the process or service to be monitored and is located in `service` directory
	
	- `ARGUMENTS`: Service runtime arguments
	
        - `CHECK_INTERVAL`: Checking interval in seconds
	
        - `BACKOFF_NUM`: Number of tries before backing off
	
        - `RESTART_ATTEPT_INTERVAL`: Seconds between tries
        
        # example:
            {
	            "SERVICE_NAME" : "echoService",
	            "ARGUMENTS" : "5 5",
	            "CHECK_INTERVAL" : "1",
	            "BACKOFF_NUM" : "5",
	            "RESTART_ATTEPT_INTERVAL" : "2"
            }

  - `service`: Includes services which should be monitored; you can create a soft link!
