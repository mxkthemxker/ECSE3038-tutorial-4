Post probe #1 
Status: 201
Number of devices: 5

Post probe #2 
Status: 201
Number of devices: 6

Put attic #1
Status: 200
Number of devices: 6

Put attic #2
Status: 200
Number of devices: 6

Delete fridge #1
Status: 200
Number of devices: 5

Delete fridge #2
Status: 404
Number of devices: 5

Post was not idempotent because sending the same request twice added another device.

Put was idempotent because sending the same request twice left the system in the same state.

Delete was idempotent because after the first request removed the device, sending it again did not change the state of the system.