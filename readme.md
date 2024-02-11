# The Portal2 Protocal
### Our Portal 2 Protocol is a system designed to host websites on a webserver close to the conventional internet. 
### What sets it apart is its capability to enable interaction among Portal 2 sites, creating a network where these sites can seamlessly communicate and pull from others to update data. 
### One of Portal2's key features is the implementation of a centralized login system, simplifying user authentication across various Portal 2 sites. Additionally, the protocol facilitates real-time updates of information between interconnected sites, ensuring that changes made on one site are reflected across the network. 
### This interconnectedness opens up new possibilities for collaboration and data exchange within the Portal 2 ecosystem, enhancing the overall user experience and functionality of the platform.


# Setup a portal

To setup a portal you can write some html code like this
```

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hello World</title>
</head>
<body>
    <h1>Hello, World!</h1>
</body>
</html>
```
You can host your file in 2 ways.

1. Giving it to sa.lex to host. This is recomended for portals not updated often as it can take up to **48 Hours** for changes to be posted.
2. Hosting html yourself. This is the other option you will host your portal using a .txt file containing your html css and js code. this html code will be displayed when someone views your site. We recommend using github pages to host your txt file

You also need a manafest for the protocall to understand what site it's looking At

Here's a JSON template for the manifest of each Portal 2 site:

```
{
  "portal_name": "MyPortal",
  "portal_permissions": {
    "accessing_portal": true,
    "user_username": true,
    "user_age": false,
    "user_dob": true,
    "user_unique_number": false
  },
  "location": {
    "type": "hosted",
    "location_code": "XXXXXX"
  },
  "other_location": {
    "type": "txt_file",
    "url": "https://example.com/portal.txt"
  },
  "portal_description": "This is a description of my Portal.",
  "portal_creator": "Alex Rose",
  "portal_date": "2024-02-10"
}
```
## Manfest Meaning:

`portal_name` The name of the Portal.

`portal_permissions`: Object containing permissions settings for the Portal.

`accessing_portal`: Whether other Portals can access this Portal.

`user_username`: Whether this portal can see it's user usernames.

`user_age` Whether this portal can see user ages.

`user_dob` Whether this portal can see user dates of birth.

`user_unique_number` Whether this portal can see the unique user numbers of the user.

`location` Object describing the hosting location.

`type` Type of hosting location (in this case, "hosted").

`location_code` Code provided by Sa.lex for hosting on their servers.

`other_location` Object describing the alternative hosting location.

`type` Type of hosting location (in this case, "txt_file").

`url` URL of the TXT file containing HTML code for rendering on the Portal.

`portal_description` Description of the Portal.

`portal_creator` Creator of the Portal.

`portal_date` Date of creation of the Portal.
