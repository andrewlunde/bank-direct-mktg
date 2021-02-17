# Python 3.9.0 on MacOSX

```
cd /Library/Frameworks/Python.framework/Versions/3.9/bin



ln -s python3.9 python



ln -s pip3 pip



ln -s python3-config python-config

ln -s easy_install-3.9 easy_install

ln -s idle3 idle

ln -s pydoc3 pydoc


# which python

/Library/Frameworks/Python.framework/Versions/3.9/bin/python

# which pip

/Library/Frameworks/Python.framework/Versions/3.9/bin/pip

python -m pip install --upgrade pip



$ tail -n 5 ~/.bash_profile

# Setting PATH for Python 3.9

# Python specific environment variables.

export PYTHONHOME=/Library/Frameworks/Python.framework/Versions/3.9

export PYTHONPATH=$PYTHONHOME/lib/python3.9

export PATH=$PYTHONHOME/bin:$PATH



# set | grep PYTHONHOME

PYTHONHOME=/Library/Frameworks/Python.framework/Versions/3.9

# set | grep PYTHONPATH

PYTHONPATH=/Library/Frameworks/Python.framework/Versions/3.9/lib/python3.9

# set | grep PATH 

PATH='/Library/Frameworks/Python.framework/Versions/3.9/bin:/Library/Frameworks/Python.framework/Versions/3.9/bin:/Users/i830671/.yarn/bin:/Users/i830671/.config/yarn/global/node_modules/.bin:/Users/i830671/Library/Python/3.7/bin:/Library/Frameworks/Python.framework/Versions/2.7/bin:/Library/Frameworks/Python.framework/Versions/3.7/bin:/usr/local/opt/make/libexec/gnubin:/usr/local/opt:/Library/Frameworks/Python.framework/Versions/3.7/bin:/Library/Frameworks/Python.framework/Versions/2.7/bin:/Users/i830671/bin:/Users/i830671/bin:/Library/Frameworks/Python.framework/Versions/3.6/bin:/Library/Frameworks/Python.framework/Versions/3.7/bin:/Applications/sap/hdbclient:/Users/i830671/git/minion:/usr/local/bin:/Library/Frameworks/Python.framework/Versions/3.7/bin:/opt/local/bin:/opt/local/sbin:/Applications/sap/hdbclient:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin:/Applications/VMware Fusion.app/Contents/Public:/usr/local/go/bin:/Library/Apple/usr/bin:/Applications/Privileges.app/Contents/Resources:/Library/Frameworks/Mono.framework/Versions/Current/Commands:/Applications/sap/xs_client/bin:/Applications/sapjvm_8/bin:/Applications/sap'

echo "hana-ml" > requirements.txt
pip install -r requirements.txt

cf create-service hana schema BANK_SCH
cf create-service-key BANK_SCH BANK_key
cf service-key BANK_SCH BANK_key

```