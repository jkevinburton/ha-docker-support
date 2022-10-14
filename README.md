


## Node-RED configuration
In order for Node-RED to be fully functional, further configuration should be done in Node-RED itself. From inside Home Assistant, click the Node-RED icon in the left bar.

* Add Home Assistant nodes to Node-RED: From the Node-RED menu on the top right bar select ‘Manage palette’, then in the install tab search for ‘node-red-contrib-home-assistant-websocket’ and install the module.
* Configure the mqtt broker: After putting an input or output mqtt node on a flow, you will be able to configure the mqtt broker in Node-RED editing the server field of the node. More info here.
* Configure connexion with Home Assistant: You need to edit an Events: all node on your workspace and fill the Home Assistant url and the access token. Information about this and how to generate an access token in Home Assistant can be found here.

* *_NOTE_*: Node-RED should be restarted for this configurations to take effect. To restart the Node-RED container execute ‘docker restart nodered’