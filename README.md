PrePark
=======

-server/backend
	-receives request from sensor with status + sensor id
	-receives request from app with status + sensor id
	-stores location of sensor in relation with sensor id, knows its status
	-handles reverse ajax requests from app to update status of parking spots

-app
	-shows a visual representation of the parking lot with green for vacant, orange for reserved, and red for full
	-sends out reverse ajax requests to server every x seconds
	-reserves parking spots for nearby users for a limited amount of time

-sensor
	-sends out status updates on status change to server
	-possibly beep? if someone else parks there
