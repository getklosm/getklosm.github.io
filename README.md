# getklosm.github.io
The Official GitHub Pages site for KLOSM, go to 'getklosm.github.io' to visit site

## how to fix known issues
if theres any issue, do these steps

### 1 - downloading python
download python 3.11.7 ( it has to be that version )

### 2 - verifing install
make sure it is on the right version by running '''python
python3 --version
''', it should return something like '''python
python 3.11.7
'''.

### 3 - installing dependencies
next run this command '''python
python3 -m pip install cryptography pygments flask flask_cors google-genai openai anthropic groq
'''

### 4 - kill any process on port 5000
run these commands based on you operating system<br>
macos / linux - '''python
kill -9 $(lsof -f -i:5000)
'''<br>
windows - open powershell as administrator, and run '''python
Stop-Process -Id (Get-NetTCPConnection -LocalPort 5000).OwningProcess -Force
'''

### 5 - relaunch the app
just open up the app, it will work ( probably )<br>
if it does not work send a email titled '''python
klosm issue report
''' to '''python
accountchair93@proton.me
''' ( you do not have to use proton to send the email )
