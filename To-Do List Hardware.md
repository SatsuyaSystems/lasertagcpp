### Request Module
	send a http post request to our server.
	Decode json data (response of our server)
### WebSocket Module
	connect to our ws
	send data in json format
	decode messages sended with tag [SERVER] (Should be used for displaying Team points in realtime)
### IR Module
	Combine necessary data that will be sent
	Decode received data
	On hit call our ws
### Update Module
	Request version and compare with current
	must be initialized and done before all other files are initialized because we prob. cant modify them when they are loaded.
	Download new data from server and replace files
	Reset device version to newest
