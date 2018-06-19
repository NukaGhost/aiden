# aiden

Aiden offers a boilerplate to start and stop services.
It also offer a basic watchdog which allow to restart the service if it fails

When you start the service it launch the service and make a pidfile under PIDFILE_LOCATION
By default, it prevents the same user to launch the same service
but you can easily modify this behavior by modifiying the variable PIDFILE_LOCATION

You need to implement at least 2 functions:
  - [service_name]_start : contains your command, must return the pid
  - [service_name]_clean : if your application needs to do some cleanup. If not just put `exit 0`

NOTE: I am a beginner in bash, so if you think something can be improved do not hesitate to tell me

COMING SOON:
  - update command
  - And i don't know what to add...
