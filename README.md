#TC-Microservice-Queue#
Docker image for TC-Queue (in teamcrop) for monitor queue and worker process queue message.

This image is based on my `voduytuan/tc-microx` image, and just only modify the `supervisord.conf` file for add programm for running workers.

The supervisord will create 30 process of `teamcrop_consumer_webhook`. 

More commands:

`supervisorctl restart all`: Restart all processes
`supervisorctl restart <<group>>:*`: Restart all processes in group <<group>>
