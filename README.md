# SF-EinsteinAnalytics-JSON-Dataflow-Commenting
A bookmarklet which allows the user to add comments to nodes within the dataflow for tracking user stories.


# To Use:
1. Copy the code from the text file and paste it into freshly made bookmark's URL
2. When you have opened up a dataflow in Einstein Analytics click on the bookmark and it will allow you to add comments to nodes by storing them using with the key "comments"

# How it works:
The bookmarklet works by running as a loop every 250ms, and checks if the user has opened a node for editing, in which case it creates the comments textblock where the user can add comments to a node.

It also checks if the user has clicked Save so that it can store the comments in a variable to be accessed when opening the "Preview JSON" window.

When the user opens the "Preview JSON" window it will update the JSON text with all newly created comments and then allow the user to download the updated JSON file with the newly created comments by replacing the the "Download JSON" button with a new one which references the updated JSON with comments.

