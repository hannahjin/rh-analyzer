# Robinhood to CSV

A Python script to export your [Robinhood](https://www.robinhood.com) trades to a .csv file. Based on the [Robinhood library by Rohan Pai](https://github.com/Jamonek/Robinhood). Read the back story on my [blog](http://www.onlineaspect.com/2015/12/17/export-robinhood-investments-to-csv).

Works on Python 2.7+ and 3.5+

#### Install:

`pip install -r requirements.txt`

#### Run:

For exporting stock trades, run:

`python csv-export.py`

For exporting options trades, run:

`python csv-options-export.py`

For Device_Token go to your browser

1. Go to robinhood.com. Log out if you're already logged in
2. Right click > Inspect element
3. Click on Network tab
4. Filter for "token"
5. With the network inspector open, login to Robinhood
6. Two new urls should appear, "api.robinhood.com" and "/oauth2/token"
7. Click the request that is not 0 bytes in size
8. Click on Headers, then scroll down to the Request Payload section
   Here, you'll see new JSON parameters for your login. What you'll need here is the device token.
