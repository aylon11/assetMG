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

Download the latests zip file under the [release](https://github.com/aylon11/assetMG/releases/tag/beta_1)) tab.
Create a folder called "assetMG" and extract the zip file to it.

0. Open Terminal and navigate to the folder where you extracted the file


1. Create a virtual environment
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

2. Install required Python packages:

  ```bash
  pip3 install -r requirements.txt
  ```

3. Run the app
  ```bash
  python3 assetMG.py
  ```
  
4. If it is your first time using assetMG, please provide relevant credentials

## Managing Universal App Campaigns' assets.

Choose an account from the accounts list on the top.
You will get a view of all the assets under that account.
Use the filter and search bars at the top to look for assets.
Once you click on an asset, you can browse the different camapiagns and adgroups and choose
to which adgroups you want to assign/remove the asset to.
Once you done, click the 'Update' button, and move on to the next asset.


