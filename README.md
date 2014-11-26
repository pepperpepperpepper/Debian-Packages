Debian-Packages
===============

Packaging files for Debian packages

<h1>Infinality Instructions</h1>

<h2>1. Clone the git repo</h2>

<span class="highlight">
git clone https://github.com/chenxiaolong/Debian-Packages.git
cd Debian-Packages/
</span>

<h2>2. Install the build dependencies. Run the following
command and install the packages it lists using apt-get/synaptic/etc.
</h2>

<span class="highlight">
cd freetype-infinality/
dpkg-checkbuilddeps
cd ../fontconfig-infinality/
dpkg-checkbuilddeps
</span>

<h2>
3. Build the packages:
</h2>

<span class="highlight">
cd ../freetype-infinality/
./build.sh
cd ../fontconfig-infinality/
./build.sh
</span>

<h2>
4. Install the deb files:
</h2>


<span class="highlight">
cd ..
sudo dpkg -i freetype-infinality/*.deb fontconfig-infinality/*.deb
</span>

You'll need to reboot after installing the deb files. Enjoy the better
looking fonts!
