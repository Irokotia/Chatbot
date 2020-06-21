## happy path
* greet
  - utter_greet
* mood_great
  - utter_happy

## sad path 1
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* deny
  - utter_soshelp
  *soshelp
      -utter_sendsos
      *responsesos
          -utter_soscall
          -utter_goodbye
  * request_repository
    - repository_form
    - form{"name": "repository_form"}
    - form{"name": null}
  * thankyou
    - utter_noworries
    -utter_goodbye

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot
