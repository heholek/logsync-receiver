# logsync-receiver

  Simple example snap to show how to receive journal messages from a device
  on a remote journal server.

  Currently only the http (not https!) protocol is supported, this will soon
  be extended.
  
  install the ```logsync-james``` snap on a machine, point it to the machine 
  running the logsync-receiver snap and remote logging should start automagically.
  
## Receiving Logs

  Log files can be found in ```/var/snap/logsync-receiver/current/```
  
  ... and can be read with:

  ```sudo journalctl -f -D /var/snap/logsync-receiver/current/```

