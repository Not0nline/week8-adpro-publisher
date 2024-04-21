# week8-adpro-publisher

7.Try to answer the following questions, and write the answer in the and new file readme.md in
you repository.  

a. How many data your publlsher program will send to the message broker in one
run?  

The publisher program will send data to the message broker five times in one run. This is because the publish_event is performed five times in the publisher.


b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber
program, what does it mean?

The URL amqp://guest:guest@localhost:5672 is the same in both the publisher and subscriber programs. This is because both are sending requests to the same RabbitMQ server. The difference lies in the result of these requests. The publisher sends messages to the queue, while the subscriber creates a listener that retrieves data from the message queue.

- sending and processing events

![img.png](img.png)

- Monitoring chart based on publisher

![img_1.png](img_1.png)

![img_2.png](img_2.png)

The image above shows that after the publisher is run, the publisher will send the hard-coded data in its code to the message queue. The subscriber, which is connected to the message queue, will receive this data from the message queue and output it to the console as per the code that has been written.

- simulation slow subscriber

![img_3.png](img_3.png)

