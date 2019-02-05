# bash
## A Daemon Supervisor which should check that the process is running and at all times and starts it in case is down. 

Input parameters:
    [
        Seconds to wait between attempts to restart service,
        Number of attempts before giving up,
        Name of the process to supervise,
        Check interval in seconds
    ]
    
It also generate logs in case of events.

__Main__ *script* is supervisor.

