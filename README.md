# Tensorflow Object Detection Walkthrough

Step 1. Clone this repository: https://github.com/nicknochnack/TFODCourse
<br/>
Step 2. Create a new virtual environment 
<pre>
python -m venv tfod
</pre> 
<br/>
Step 3. Activate your virtual environment
<pre>
source tfod/bin/activate # Linux
.\tfod\Scripts\activate # Windows 
</pre>
<br/>
Step 4. Install dependencies and add virtual environment to the Python Kernel
<pre>
python -m pip install --upgrade pip
pip install ipykernel
python -m ipykernel install --user --name=tfodj
</pre>
<br/>
Step 5. Run through the notebook, ensuring your collected images are in the train and test folders


Bucket Cors Config Command 
<pre>
ibmcloud cos bucket-cors-put --bucket nickstfjs --cors-configuration file://corsconfig.json
</pre>

<br/>
<br/>
CORS Config Setup
<pre>
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
</pre>

