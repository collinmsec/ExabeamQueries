``` 
  ______           _                           ____                  _           
 |  ____|         | |                         / __ \                (_)          
 | |__  __  ____ _| |__   ___  __ _ _ __ ___ | |  | |_   _  ___ _ __ _  ___  ___ 
 |  __| \ \/ / _` | '_ \ / _ \/ _` | '_ ` _ \| |  | | | | |/ _ \ '__| |/ _ \/ __|
 | |____ >  < (_| | |_) |  __/ (_| | | | | | | |__| | |_| |  __/ |  | |  __/\__ \
 |______/_/\_\__,_|_.__/ \___|\__,_|_| |_| |_|\___\_\\__,_|\___|_|  |_|\___||___/
                                                                                 
                                                                                 
```     

# ExabeamQueries
                                                                
A collection of Exabeam queries to be used for threat hunting & detection.

I encourage any contribution of hunting/detection rules to the respository and would love to collaborate on some queries! If you are interested in contributing a query, please open a pull request.

*Note: Some of the fields being used in published queries may differ in your environment depending on parsing used in the Exabeam instance. Please test these queries in your environment/Exabeam instance.*
## Log Sources: 
The queries in this repository will be querying data from below log sources: 

| Log Source |
| ----------- |
| AWS Cloudtrail |
| Microsoft 365 |
| Windows | 
| Linux | 
| Okta | 

## Contributing
Please use pull requests for submitting changes to the ExabeamQueries repository. 

Pull requests can be submitted directly through the web interface on Github, this is the easiest way to go about submitting new query or a change to a query.

When creating a new file in a directory, or editing a file already in place, you can commit the changes via a button on the web interface. When this is clicked, you will have the option to "Create a new branch for this commit and start a pull request". This is my preffered way of opening pull requests. 

Link to Github pull request Guide: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request

Mandatory items for inside the file containing the query: 
* The following text: NOTE: Some of the fields that are being used may be different in your environment depending on parsing.
* A short text note, with the name of the query/what it does. This should be similar to the name of the file you are creating/editing.
* The query itself. 
* Inspiration/Reference at the bottom of the file, if relevant. We want to credit others for work thay may have performed even if their rule was written in a different query language.

If there are any questions around this process I am happy to help and give guidance!
