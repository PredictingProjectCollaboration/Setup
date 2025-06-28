# Stragic Execution 


# React app
- create a form for upload file dataset (accept csv or json)
    + upload file fields
    + select which column/field is "Target fields" (the rest are Features)
    + Error notification alert

- Displaying area for displaying chart (visuallization) (connect to MongoDB service)

- An area for chat bot (send request to SpringAIapp )

# Flaskapp
- A Controller to receive file upload request (from React app), then save dataset 
    + into Redis by session (for anonymous user).
    + into MongoDB for logged in user.

    -> Request from Reactapp will also include list of columns/fields which is determined as "Target fields" of Dataset
    -> Trigger the Helper class to run prediction
        - A Helper class to execute prediction
            -> trigger function by invoking python file to run predicting model on uploaded dataset
            -> use model to provide prediction and return output to invoking Controller


- A Controller for user registry  -> Data user saved in SQLite

- A Controller for user logging in  -> Data user saved in SQLite

# MongoDB
- use for Registered and Logged in user
- Save logged in user's dataset and provide analisys via SDK and REST API

# Redis
- use for anonymous user
- Persist dataset by session

# SpringAIapp
- Connect to MongoDB to memorize dataset as context
- A service receive request from chat bot (Reactapp) and send back response

