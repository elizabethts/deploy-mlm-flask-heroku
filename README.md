# Deploy ML model with Flask to Heroku

Click the button below to quickly clone and deploy into your own Heroku acount.
If you don't have one it'll prompt you to setup a free one.

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

Once deployed to your Heroku instance run the following:

```bash
curl -s -XPOST 'https://<name-of-your-heroku-app>.herokuapp.com/' -d '{"Pclass":3,"Age":2,"SibSp":1,"Fare":50}' -H 'accept-content: application/json'
```

Alternatively a simple python script:

```python
import requests
import json
url = 'https://<name-of-your-heroku-app>.herokuapp.com/'
data = {"Pclass":3, "Age":2, "SibSp":1, "Fare":50}
response = requests.post(url, json.dumps(data))
print(response.json())
```

# Article

You can read the full article that was published on Towards Data Science

 - **Article**: [Towards Data Science: Create an API to Deploy Machine Learning Models using Flask](https://towardsdatascience.com/create-an-api-to-deploy-machine-learning-models-using-flask-and-heroku-67a011800c50)
 - **Author**: [Elizabeth Ter Sahakyan](https://towardsdatascience.com/@liztersahakyan)

# Acknowlegements
Thank you to [Josh Peak](https://github.com/neozenith) who added the button for heroku deployment
