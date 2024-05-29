<h3 id="bkmrk-1.-install-git">1. Install Git</h3>
<h4 id="bkmrk-using-homebrew-%28reco">Using Homebrew (recommended):</h4>
<ol id="bkmrk-install-homebrew-%28if">
<li>
<p><strong>Install Homebrew</strong> (if you don't have it already): Open Terminal and run:</p>
<pre><code class="language-">/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"</code></pre>
</li>
<li>
<p><strong>Install Git</strong>: Run the following command in Terminal:</p>
<pre><code class="language-">brew install git</code></pre>
</li>
</ol>
<h4 id="bkmrk-alternatively%2C-using">Alternatively, using Xcode Command Line Tools:</h4>
<ol id="bkmrk-open-terminal-and-ru">
<li>Open Terminal and run:
<pre><code class="language-bash">xcode-select --install</code></pre>
</li>
<li>Follow the on-screen instructions to complete the installation.</li>
</ol>
<h3 id="bkmrk-2.-configure-git">2. Configure Git</h3>
<ol id="bkmrk-set-your-name-and-em">
<li>
<p><strong>Set your name and email</strong>:</p>
<pre><code class="language-bash">git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"</code></pre>
</li>
<li>
<p><strong>Check the configuration</strong>:</p>
<pre><code class="language-bash">git config --list</code></pre>
</li>
</ol>
<h3 id="bkmrk-3.-connect-to-a-git-">3. Connect to a Git Hosting Service</h3>
<h4 id="bkmrk-github-%28example%29%3A">GitHub (example):</h4>
<ol id="bkmrk-create-a-github-acco">
<li>
<p><strong>Create a GitHub account</strong>: If you don't already have one, sign up at <a href="https://github.com/" target="_new" rel="noreferrer">github.com</a>.</p>
</li>
<li>
<p><strong>Generate an SSH key</strong>:</p>
<pre><code class="language-bash">ssh-keygen -t ed25519 -C "your.email@example.com"</code></pre>
<p>Press Enter to accept the default file location, and set a passphrase if desired.</p>
</li>
<li>
<p><strong>Add the SSH key to your GitHub account</strong>:</p>
<ul>
<li>Copy the SSH key to your clipboard:
<pre><code class="language-bash">pbcopy &lt; ~/.ssh/id_ed25519.pub</code></pre>
or
<pre><code class="language-bash">cat ~/.ssh/id_ed25519.pub</code></pre>
<br><br>
<ul>
<li>Go to your GitHub account settings, navigate to <strong>SSH and GPG keys</strong>, and click <strong>New SSH key</strong>. Paste the key and give it a title.</li>
</ul>
</li>
</ul>
</li>
<li>
<p><strong>Test your SSH connection</strong>:</p>
<pre><code class="language-bash">ssh -T git@github.com</code></pre>
<p>You should see a success message.</p>
</li>
</ol>
<h3 id="bkmrk-4.-clone-a-repositor">4. Clone a Repository</h3>
<ol id="bkmrk-clone-a-repository%3A-">
<li><strong>Clone a repository</strong>:
<pre><code class="language-bash">git clone git@github.com:username/repository.git</code></pre>
</li>
</ol>
<h3 id="bkmrk-5.-basic-git-command">5. Basic Git Commands</h3>
<ul id="bkmrk-check-status%3A-git-st">
<li>
<p><strong>Check status</strong>:</p>
<pre><code class="language-bash">git status</code></pre>
</li>
<li>
<p><strong>Add changes</strong>:</p>
<pre><code class="language-bash">git add .</code></pre>
</li>
<li>
<p><strong>Commit changes</strong>:</p>
<pre><code class="language-bash">git commit -m "Your commit message"</code></pre>
</li>
<li>
<p><strong>Push changes</strong>:</p>
<pre><code class="language-bash">git push</code></pre>
</li>
</ul>
<p id="bkmrk-following-these-step">Following these steps will set you up with Git on your Mac and enable you to interact with remote repositories.</p>
