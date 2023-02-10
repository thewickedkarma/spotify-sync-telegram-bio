# spotify-sync-telegram-bio
A code snippet to sync your currently playing song on Spotify and your current Telegram bio. 

# Getting Started

## Telegram credentials

* Grab your Telegram API ID and API HASH from https://my.telegram.org/auth

* Go to "API development tools" and fill out the form.

* You will get basic addresses as well as the api_id and api_hash parameters required for user authorization.

* For the moment each number can only have one api_id connected to it.

* Copy these credentials for later

## Spotify Credentials

* Visit https://spotify-github-profile.vercel.app/api/login

* Login using Spotify

* Grab the uid( highlighted text in ss ) from the link that appears as shown below in the screenshot

![Spotify SS](http://0x0.st/Hro2.png)

* Copy this for later use

## Next Steps

* Fork this Repository

* Open update.py and paste the credentials into their respective variables

``` 

#get these api values from telegram website

api_id = your telegram api id here #don't use quote
api_hash = "paste your api hash"

#Spotify api uid
uid="paste your uid"

```

## All set, just a few extra steps

* Clone the repository you just forked 

```
git clone https://github.com/your-username/your-repo-name.git
```

* Run the setup (update.py) locally on your PC or use google colab

```
pip install -r requirements.txt

python3 update.py

```

* Follow the instructions in your terminal/python editor.

* After logging in successfully, you will notice a file named ```user.session``` in the cloned folder.

* Upload that file to your forked github repo

## Deploying it on cloud

* Use https://railway.app to deploy your repository to the cloud 

* Connect your github account and deploy the repo, the deployment will be handled automatically by Procfile worker

## End notes

This is a trivial code snippet I wrote in 5 minutes for fun; it's definitely not pretty, and code improvement is always welcome

The code checks for update every 15s, if the same song is playing, it doesn't update. 





