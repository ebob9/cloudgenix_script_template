# cloudgenix_script_template
Quick starter script for making command line scripts using CloudGenix Python SDK

* `my_script.py` - example, modifiable script
* `cloudgenix_settings.py.example` - example of a cloudgenix_settings.py authentication file.

the `my_script.py` looks for the following for AUTH, in this order of precedence:
1. `--email` or `--password` options on the command line.
2. CLOUDGENIX_USER and CLOUDGENIX_PASSWORD values imported from `cloudgenix_settings.py`
3. CLOUDGENIX_AUTH_TOKEN value imported from `cloudgenix_settings.py`
4. X_AUTH_TOKEN environment variable
5. AUTH_TOKEN environment variable
6. Interactive prompt for user/pass (if one is set, or all other methods fail.) 
