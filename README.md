# library_management

## Quick start
to start Flask sever:
```bash
$ flask run
```
to start Celery asynchronous task queue:
```bash
$ celery -A tasks worker --loglevel=info
```

### What's next?
After starting all services you can request to server

#### Start new task

* localhost:5000/start_task -> if you request this route, new task _starts_ and your unique **task_id** returns

#### Check status of task out

* localhost:5000/task_status/<task_id> -> if you request this route with your unique **task_id** it returns _status_ of your task

#### Check result of task out

* localhost:5000/task_result/<task_id> -> if you request this route with your unique **task_id** it returns _result_ of your task

 

