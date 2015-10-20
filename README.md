## Netscaler WAF Security for Splunk ##

### Overview ###

The app "Netscaler WAF Security for Splunk" analyzes attacks on your web infrastructure prohibited by Netscaler. It's is a fork of the original F5 WAF Security by Nexinto located at https://splunkbase.splunk.com/app/2873.

Features:

- Displays attacks based on GeoIP
- Displays attacks based on Type
- Displays attacks based on Country
- Displays attacks based on IPs
- Heatmap for Attack Type Distribution by Type, Country, Violation
- Security Stats table for displaying chronological attack requests and locations

### Installation ###

Deploy "Netscaler WAF Security for Splunk" like every other App by uploading  it using the WebGUI or extracting it to $SPLUNK_HOME$/etc/apps. 
Restart Splunk afterwards.

In a distributed environment the app has to be deployed to every Search head and Indexer. Make sure the app is also deployed on the Host or 
Forwarder receiving the events from the Netscaler devices. 

With default settings the app will create an index named “netscaler” and a TCP input on port 10005 using sourcetype citrix:netscaler. You can customize these 
settings by changing the TCP port in inputs.conf.

The app have been tested against Splunk v6.1, v6.2 and v6.3. Lower versions will not work "out of the box". The Common Event Format (CFE) descripted in http://support.citrix.com/article/CTX136146
is supported but not a requirement. 

### Feedback and Contact ###

If you have Feedback, issues or questions please use issue tracker at Github page: http://github.com/schose/netscaler_waf .

For direct Feedback please contact: andreas@batchworks.de. 

This app was created by:

Andreas Roth
Batchworks
Strehlener Strasse 14
01069 Dresden

Internet: www.batchworks.de