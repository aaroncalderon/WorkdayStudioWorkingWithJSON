# Workday Studio Working with JASON Arrays Sample Project

The purpose of this repo is to show how to handle JSON arrays inside Workday Studio.

This project loads a JSON file and then it outputs the value of an array property.

## How to use?

Once you import the project into eclipse, feel free to deploy and run the integration.

The key step is the log labeled __Log_Step1p2__. It shows how to get to the array.

```mvel
# 
Step 1.2

# messages
@{props['messages'] = props['jsonObject'].getJSONArray("messages")}

# message 1
@{props['messages'].get(0)}

# message 1
@{props['messages'].length()}

```

## How to import project into eclipse?

1. Clone this repo into your Workday's workspace
2. On Workday Studio select __File > Import...__
3. Select __General > Existing Projects into Workspace__ and click __Next__
4. Choose either __Select root directory or Select archive file__ and click the associated __Browse__ to locate the directory or file containing the projects.
5. Under __Projects__ select the project or projects which you would like to import.
6. Click __Finish__ to start the import.

## Reference

[Eclipse > Importing existing projects](https://help.eclipse.org/kepler/index.jsp?topic=%2Forg.eclipse.platform.doc.user%2Ftasks%2Ftasks-importproject.htm)
