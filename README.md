

Cors Config: ibmcloud cos bucket-cors-put --bucket nickstfjs --cors-configuration file://corsconfig.json

cors.config file
{
"CORSRules": [
{
"AllowedHeaders": ["*"],
"AllowedMethods": ["GET"],
"AllowedOrigins": ["*"]
}
]
}

<pre>
python -m venv tfod
Mac: source tfod/bin/activate
Windows: .\tfod\Scripts\activate
python -m pip install --upgrade pip
pip install ipykernel
python -m ipykernel install --user --name=tfodj
pip install -r requirements.txt --use-deprecated=legacy-resolver
deactivate
jupyter kernelspec list
jupyter kernelspec uninstall myenv
</pre>