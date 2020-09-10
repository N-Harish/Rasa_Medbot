
## search hospital path 1
* greet
  - utter_how_can_i_help
* search_provider{"facility":"hospital"}
  - utter_ask_location
* inform{"location":"San Francisco"}
  - action_facility_search
  - slot{"address":"MGM Hospital Kamothe, Near Sion-Panvel Highway"}
* thanks
  - utter_goodbye

## search hospital path 2
* greet
  - utter_how_can_i_help
* search_provider{"facility":"hospital","location":"San Francisco"}
  - action_facility_search
  - slot{"address":"MGM Hospital Kamothe, Near Sion-Panvel Highway"}  
* thanks
  - utter_goodbye            


## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot
