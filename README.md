# common-linux-commands-to-manage-web-server
i'm not a server admin by profession and have to google every time i want to manage server via ssh. So i'm creating this repo to log all commands which i run on my server

 
<h3>Install Nano</h3>
<code>sudo yum install nano</code>

<h3>get file or directory size</h3>
<code>sudo du -sh /var</code>

<h3>zip a file or folder</h3>
<code>zip -r[flag for folders] zip-file-name folder-to-be-zipped</code>
<code>zip -r httpdocs.zip httpdocs</code>

<h3>disable root login</h3>
<p>Go to the following file. Edit it and set [PermitRootLogin] to no. if its commented out, remove # sign. Then restart ssh service</p>
<code>PermitRootLogin no</code>
<code>systemctl restart sshd</code>
