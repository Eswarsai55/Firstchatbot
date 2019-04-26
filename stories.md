## greet
* greet
    - utter_greet

## thank
* thank
    - utter_thank

## bye
* bye
    - utter_goodbye
	
## App not working
* greet
    - utter_greet
* app_issue
	- slot{"requested_slot": "application"}
	- utter_ask_application
* inform{"application": "google"}
	- slot{"requested_slot": "description"}
	- utter_ask_description
* inform{"description": "internet issue"}
	- utter_solution
* thank
    - utter_thank
* bye
    - utter_goodbye

## Url not working
* greet
    - utter_greet
* url_issue
	- slot{"requested_slot": "url"}
	- utter_ask_url
* inform{"url": "www.google.com"}
	- slot{"requested_slot": "description"}
	- utter_ask_description
* inform{"description": "internet issue"}
	- utter_solution
* thank
    - utter_thank
* bye
    - utter_goodbye