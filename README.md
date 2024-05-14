# Nessus-Combiner-Parser

There are a few other projects for this task. But I needed some detailed functions such as repeating vulnerabilities, combining multiple Nessus files, and customizable columns.

If you are work with multiple teams in a company or foundation, when you wanted to share the scan result they usually expect excel or pdf files :smile: . Because they need to move one by one, line by line. This tool can provide such functions:

###### You can track repeating vulnerabilities. For example, server got Apache 2.1.1 at port 8080 web service. You will have more than 10 vulnerabilities for each version until the latest one suggested. There will be an excel page with "Repeating" name. If a host:port has multiple vulnerability with same topic you can see it at "Repeating" page. Pick one, put an "x" and leave others as "0".
###### There are preselected plug-in lists at code. You can edit them if want to select them to inform other teams, just add the plugin name at write array. If don't want them to exist at the final result, just put "0". For example, you don't need "self-signed certificate" vulnerability at local area network tests. However, if you are scanned from an outside network, it should have been taken care of. 

1. `git clone https://github.com/esenturq/nessus-combiner-parser.git`
2. `python3 -m pip install -r requiremests.txt`
3. `sudo python3 NessusCombinerParser.py`
4. select the Nessus files and push "analyze" button


[![UI](https://ibb.co/1LpmS8b "UI")](https://ibb.co/1LpmS8b "UI")
