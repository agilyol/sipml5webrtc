#webrtc for frameworks
The file content simple javascript functions for making calls from the web with using webrtc. I created application base of sipml5 api.

	Application Requirements:

* Asterisk
* To properly work of webrtc the port number 8089 should be accessible.
* Should work with any browser from the list http://iswebrtcreadyyet.com/, but preference is Google chrome.

Note:  The main js file is sipcall.js which should use for backend part.

     
     Settings:

Paramaters in below should be pass from backend programming language or framework:

* Disname - User display name
* PrivIdentity - User name or private identity 
* PubIdentity - Public identity 
* Txtpas - User password for connecting to network
* Pnumber - Receiver number or Number which user should call

Note: All parameters have default value which was used for test purpose.

	 Functions:
* sipRegister() - use for sign in
* sipunRegister() - use for logout
* sipCall() - use for calling
* sipMute() - use for muting call
* sipunMute() - use for unmute call
* sipHold() - use for hold in line
* sipResume() - use for Resuming call
* sipTransfer() - use for transfer call

Note: To discontinue (stop) incoming calls you should need to create button with id btnAccept. 
txtCallStatus - is label id and it can be replaced with span. 
The order of js file loading should be same in newembed.htm. The audios file should be use as html tags (These parameters are invisible) . 
Credentials should be load as in below:
loadCredentials(Disname,PrivIdentity, PubIdentity, TxtPas);	
To comparing original file this version can be use in frameworks like Phoenix or Flask.
