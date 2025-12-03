<h1>Multi-Person Face Recognition System</h1>

<h2>1. Overview</h2>
<p>
This project is a real-time multi-person face recognition system built using Python, OpenCV, dlib, and Flask. 
It detects and recognizes multiple faces simultaneously from a webcam or video file and streams the processed 
output through a browser interface. Facial embeddings are generated using dlib’s 128-dimensional face encoding 
model and matched against stored known encodings. The project was developed as part of AIML training and 
enhanced with real-time inference, webcam integration, and modular structure.
</p>

<h2>2. Features</h2>
<ul>
  <li>Real-time face detection and recognition</li>
  <li>Supports webcam and video input</li>
  <li>Generates facial embeddings from training images</li>
  <li>Flask-based dashboard for live streaming</li>
  <li>Modular and clean code architecture</li>
  <li>Easily extendable for multi-camera systems</li>
</ul>

<h2>3. Project Architecture</h2>
<ol>
  <li>Training images are processed to generate facial embeddings.</li>
  <li>Embeddings are saved into a serialized file for matching.</li>
  <li>The real-time recognition script captures video frames.</li>
  <li>Faces are detected and converted into embeddings.</li>
  <li>Embeddings are compared with stored encodings.</li>
  <li>Processed video frames are streamed through Flask.</li>
</ol>

<h2>4. Tech Stack</h2>
<ul>
  <li>Python</li>
  <li>OpenCV</li>
  <li>dlib</li>
  <li>face_recognition library</li>
  <li>Flask</li>
  <li>Pandas</li>
  <li>HTML and CSS</li>
</ul>

<h2>5. Folder Structure</h2>
<pre>
Multi-Person-Face-Recognition/
│
├── src/
│   ├── app.py
│   ├── dlib_face_recognition.py
│   ├── dlib_face_embeddings.py
│   ├── database_pandas.py
│   ├── parameters.py
│   ├── custom_logging.py
│   ├── locks.py
│   └── util/
│
├── templates/
│   └── index.html
│
├── static/
│   ├── css/
│   │   └── styles.css
│   └── images/
│
├── requirements.txt
├── README.md
└── .gitignore
</pre>

<h2>6. Installation</h2>

<h3>Step 1: Clone the repository</h3>
<pre>
git clone https://github.com/yourusername/Multi-Person-Face-Recognition.git
cd Multi-Person-Face-Recognition
</pre>

<h3>Step 2: Create a virtual environment</h3>
<pre>
python3 -m venv myenv
source myenv/bin/activate
</pre>

<h3>Step 3: Install dependencies</h3>
<pre>
pip install -r requirements.txt
</pre>

<h2>7. How It Works</h2>

<h3>Generating Embeddings</h3>
<ol>
  <li>Add images of each person inside separate folders in the dataset directory.</li>
  <li>Run the embedding script to generate encodings.</li>
</ol>
<pre>
python3 src/dlib_face_embeddings.py
</pre>

<h3>Real-Time
