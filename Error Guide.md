<b>Error:</b> No module named ‘xxxxxx’<br/>
<b>Solution:</b> Install that module
<pre>!pip install xxxxxx</pre>

<i>Example:</i><br/>
Error: No module named typeguard<br/>
Solution: pip install typeguard  # note the name of the module will not always equal the package name

<b>Error:</b> AttributeError: module 'sip' has no attribute 'setapi'<br/>
<b>Solution:</b> Downgrade matplotlib to version 3.2 by running the following command
<pre>!pip install matplotlib==3.2</pre>

<b>Error:</b> ValueError: numpy.ndarray size changed, may indicate binary incompatibility. Expected 88 from C header, got 80 from PyObject<br/>
<b>Solution:</b>  Reinstall pycocotools
<pre>Pip uninstall pycocotools -y
Pip install pycocotools</pre>

<b>Error:</b> ValueError: 'images' must have either 3 or 4 dimensions.<br/>
<b>Solution:</b> Restart your jupyter notebook as the Webcam is unavailable. If using images, this normally means your image name and path is incorrect.

<b>Error:</b>error: (-2:Unspecified error) The function is not implemented. Rebuild the library with Windows, GTK+ 2.x or Cocoa support. If you are on Ubuntu or Debian, install libgtk2.0-dev and pkg-config, then re-run cmake or configure script in function 'cvDestroyAllWindows'<br/>
<b>Solution:</b> Reinstall opencv and uninstall opencv-headless
<pre>
pip uninstall opencv-python-headless -y
pip install opencv-python --upgrade
</pre>

<b>Error:</b>When running GenerateTFRecords script you receive an error like the following:
  File "Tensorflow\scripts\generate_tfrecord.py", line 132, in create_tf_example
    classes.append(class_text_to_int(row['class']))
  File "Tensorflow\scripts\generate_tfrecord.py", line 101, in class_text_to_int
    return label_map_dict[row_label]
KeyError: 'ThumbsDown' # YOUR LABEL HERE
 <br/>
<b>Solution:</b> This is likely because you mismatches between your annotations and your labelmap. Ensure that the label names from your annotations match the label map exactly, note it is case sensitive. 

<b>Error:</b>When running training script from the command line, you get a No module error. e.g. ModuleNotFoundError: No module named 'cv2'
 <br/>
<b>Solution:</b> Remember you need to activate your environment at the command line in order to leverage all the packages you have installed in it. 

<b>Error:</b> When training, only the CPU is used and the GPU is ignored. 
<br/>
<b>Solution:</b> Ensure you have a matching CUDA and cuDNN version for your Tensorflow version installed. Windows:https://www.tensorflow.org/install/source_windows, Linux/macOS: https://www.tensorflow.org/install/source

<b>Error:</b>CUBLAS_STATUS_ALLOC_FAILED or CUDNN_STATUS_ALLOC_FAILED <br/>
<b>Solution:</b> This is because the available VRAM on your machine is completely consumed and there is no more memory available to train. Quit all of your Python programs and stop your Jupyter Notebook server to free up the VRAM and run the command again. 



Template
<b>Error:</b> <br/>
<b>Solution:</b> 
<pre></pre>