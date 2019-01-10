## Installation

### for mac

```
cd ~/Library/Application Support/Franz/recipes
mkdir dev
cd dev
git clone git@github.com:tomoyamachi/recipe-franz-awsconsole.git
```

and restart Franz.

Only support owner signin.
Not support IAM user signin.


### for IAM user signin

edit package.json

```
- "serviceURL": "https://signin.aws.amazon.com/console",
+ "serviceURL": "https://{teamID}.signin.aws.amazon.com/console",
+ "hasTeamID": true,
```

and restart Franz.
