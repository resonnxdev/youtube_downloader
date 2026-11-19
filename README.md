<h1>YouTubeDownloader</h1>

<p>An open-source project. No more searching all over the internet for ways to download videos or music from YouTube — just follow a few simple steps and you'll have your own service right at your fingertips!</p>

<hr>

<h2>Requirements</h2>

<table>
<tr>
  <th>Name</th>
  <th>Version</th>
  <th>Description</th>
</tr>
<tr>
  <td>FFmpeg</td>
  <td>2025-12-18 and higher</td>
  <td>For conversion</td>
</tr>
<tr>
  <td>Python</td>
  <td>3.12+</td>
  <td>Server logic and working with FFmpeg</td>
</tr>
</table>

<hr>

<h2>Installation</h2>

<h3>Windows</h3>

<ol>
<li>
  <strong>Install Python</strong>
  <p>Download and install Python 3.12+ from the official website: <a href="https://www.python.org/downloads/">https://www.python.org/downloads/</a></p>
  <blockquote>
    <p>⚠️ During installation, make sure to check <strong>"Add Python to PATH"</strong>.</p>
  </blockquote>
  <p>Verify the installation:</p>
  <pre><code>python --version
</code></pre>
</li>

<li>
  <strong>Install dependencies</strong>
  <p>Open a terminal in the project folder and run:</p>
  <pre><code>pip install -r requirements.txt
</code></pre>
</li>

<li>
  <strong>Install FFmpeg</strong>
  <ul>
    <li>Download the build from <a href="https://www.gyan.dev/ffmpeg/builds/">https://www.gyan.dev/ffmpeg/builds/</a> (or <a href="https://ffmpeg.org/download.html">https://ffmpeg.org/download.html</a>).</li>
    <li>Extract the archive and add the <code>bin</code> folder to your system <strong>PATH</strong>.</li>
    <li>Verify:
      <pre><code>ffmpeg -version
</code></pre>
    </li>
  </ul>
</li>
</ol>

<h3>macOS</h3>

<blockquote>
<p>⚠️ <strong>Homebrew is required.</strong> If you don't have it installed, run the following command in Terminal:</p>
<pre><code>/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
</code></pre>
</blockquote>

<ol>
<li>
  <strong>Install Python</strong>
  <pre><code>brew install python
</code></pre>
  <p>Verify:</p>
  <pre><code>python3 --version
</code></pre>
</li>

<li>
  <strong>Install dependencies</strong>
  <p>Open Terminal in the project folder and run:</p>
  <pre><code>pip3 install -r requirements.txt
</code></pre>
</li>

<li>
  <strong>Install FFmpeg</strong>
  <pre><code>brew install ffmpeg
</code></pre>
  <p>Verify:</p>
  <pre><code>ffmpeg -version
</code></pre>
</li>
</ol>

<hr>

<h2>Running</h2>

<blockquote>
<p>⚠️ <strong>An active internet connection is required</strong> for the service to work (downloading and converting videos).</p>
</blockquote>

<ol>
<li>
  <strong>Start the server</strong>
  <pre><code>python app.py
</code></pre>
</li>

<li>
  <strong>Open the service in your browser</strong>
  <p>Go to the address shown in the terminal — usually:</p>
  <pre><code>http://127.0.0.1:7070
</code></pre>
</li>
</ol>

<h3>Access from other devices (LAN / Radmin VPN)</h3>

<p>The service is available to all users on your local network.</p>

<ul>
<li>
  <strong>Local network:</strong> connect using the machine's local IP, e.g. <code>http://192.168.XX.XX:7070</code> (use the IP shown in your system's network settings).
</li>
<li>
  <strong>Radmin VPN:</strong> use the IP shown in the Radmin VPN app, appending the port <code>7070</code>, e.g. <code>http://26.XX.XX.XX:7070</code>.
</li>
</ul>