# Exchange

Multiple different exchange types:

- nameless:

	- routes without a routing key

- fanout:

	- routes a received message to all queues bound to it
	- ignores routing key

- direct:

	- routes received message to the queue using a routing key

- topic:

	- queues have binding key patterns
	- received messages are forwarded to matching queues

- headers:

	- queues have binding key patterns
	- message headers are compared against key patterns
	- special header `x-match` determines behaviour
	- message delivered to all matching 
