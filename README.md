# assetMG

Centralized asset management platform for UAC

**This is not an officially supported Google product.**

Contact: eylong@google.com

## Why?

Creative assets are only accessible in the Ad-group level, 
Which makes managing UAC assets a manual job and creates significant overhead.

## What?

Easily add, change or remove creative assets across different ad groups and campaigns.


## Requirements

- Python 3.6+
- Access to AdWords API (refer to
  [Apply for access to the AdWords API](https://developers.google.com/adwords/api/docs/guides/signup)).
- OAuth 2 credentials (refer to
  [Generate OAuth2 credentials](https://developers.google.com/adwords/api/docs/guides/authentication#create_a_client_id_and_client_secret)).
  

## Setup

Download the latests zip file under the 'release' tab.

0. Optional step: consider using
[virtualenv](https://virtualenv.pypa.io/en/latest/) to isolate the Python
environment and libraries:

  ```bash
  python3 -m venv .venv
  ```
  then, for mac/linux:
  ```bash
  . .venv/bin/activate
  ```  
  for windows:
  ```bash
  .venv\Scripts\activate.bat
  ```  

1. Install required Python packages:

  ```bash
  pip3 install -r requirements.txt
  ```

2. Edit `config.yaml` and replace placeholders with your Google Ads
  account ID, OAuth 2 credentials, and developer token.
  
3. Acquire OAuth 2 refresh token running the script with `-a` option and
  following on-screen prompts:
  (You only need to do it the first time you are using)
  ```bash
  python3 app.py -a
  ```

4. Run the app
  ```bash
  python3 app.py
  ```
  
5. Open your browser, and go to 127.0.0.1:5000


## Managing Universal App Campaigns' assets.

Choose an account from the accounts list on the top.
You will get a view of all the assets under that account.
once you click on an asset, you can browse the different camapiagns and adgroups and choose
to which adgroups you want to assign/remove the asset to.
Once you done, click the 'Update' button, and move on to the next asset.

