[![Sync Garmin to Notion](https://github.com/chloevoyer/garmin-to-notion/actions/workflows/manual.yml/badge.svg?branch=main)](https://github.com/chloevoyer/garmin-to-notion/actions/workflows/manual.yml)
# Garmin to Notion Integration :watch:
This project connects your Garmin activities and personal records to your Notion database, allowing you to keep track of your performance metrics in one place.

## Features :sparkles:  
- Automatically sync Garmin activities to Notion.
- Extract Garmin personal records such as fastest 1K and longest ride.
- Easy setup with clear instructions and minimal coding required.

## Prerequisites :hammer_and_wrench:  
- A Notion account with API access.
- A Garmin Connect account to pull activity data.
- If you wish to sync your Peloton workouts with Garmin, see [peloton-to-garmin](https://github.com/philosowaffle/peloton-to-garmin)
## Getting Started :dart:
Follow these steps to set up the integration:
### 1. Set Environment Secrets
Ensure that your environment secrets are correctly configured for secure data access.
### 2. Create Notion Token
* Go to [Notion Integrations](https://www.notion.so/profile/integrations).
* [Create](https://developers.notion.com/docs/create-a-notion-integration) a new integration and copy the integration token.
* [Share](https://www.notion.so/help/add-and-manage-connections-with-the-api#enterprise-connection-settings) the integration with the target database in Notion.
### 3. Run Scripts (if not using automatic workflow)
* Run [garmin-activities.py](https://github.com/chloevoyer/garmin-to-notion/blob/main/garmin-activities.py) to sync your Garmin activities to Notion.  
`python garmin-activities.py`
* Run [person-records.py](https://github.com/chloevoyer/garmin-to-notion/blob/main/personal-records.py) to extract activity records (e.g., fastest run, longest ride).  
`python personal-records.py` 
## Example Configuration :pencil:    
You can customize the scripts to fit your needs by modifying environment variables and Notion database settings.  

Here is a screenshot of what my Notion dashboard looks like:  
![garmin-to-notion_demo](https://github.com/user-attachments/assets/b398c896-1142-41ac-bc4b-687b6641c50f)

My Notion template is available for free and can be duplicated to your Notion [here](https://www.notion.so/chloevoyer/Fitness-Tracker-Template-4b4ce8b4f0c349228605382be3c5623b?pvs=4)

## Acknowledgements :raised_hands:  
- Reference dictionary and examples can be found in [cyberjunky/python-garminconnect](https://github.com/cyberjunky/python-garminconnect.git).
- This project was inspired by [n-kratz/garmin-notion](https://github.com/n-kratz/garmin-notion.git).
## Contributing :handshake:   
Contributions are welcome! If you find a bug or want to add a feature, feel free to open an issue or submit a pull request. Financial contributions are also greatly appreciated :blush:    

<a href="https://www.buymeacoffee.com/cvoyer" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>   

## :copyright: License  
This project is licensed under the MIT License. See the LICENSE file for more details.


