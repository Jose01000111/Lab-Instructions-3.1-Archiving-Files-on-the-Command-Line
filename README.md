### 🧪 Lab Instructions — 3.1 Archiving Files on the Command Line

---

>💬 **Tip:** Paste this study guide into ChatGPT and ask for **more instructions** by specifying:  
>- “Provide step-by-step lab instructions for this objective.”  
>- “Include which Linux distro to use (Debian/Ubuntu or RHEL/Fedora).”  
>- “Show examples of installing, verifying, and managing desktop and server applications.”  
>- “Include minimal command-line practice for package management and development tools.”  
>- “Focus only on what is most important for passing the LPI Linux Essentials exam.”  

>This will prompt ChatGPT to give **practical, exam-focused lab steps** for each section.

---

**Objective:** Practice archiving and compressing files in your home directory.  

**Steps:**  

1. 📁 **Create a test directory**  
   - Run: `mkdir ~/archive_lab`  
   - Move into it: `cd ~/archive_lab`  

2. 📝 **Create some test files**  
   - `touch file1.txt file2.txt file3.txt`  

3. 🛠️ **Archive files using `tar`**  
   - `tar -cvf myarchive.tar file1.txt file2.txt file3.txt`  
   - **Explanation:** Creates a `.tar` archive, verbose output shows included files  

4. 🔧 **Compress archive using `gzip`**  
   - `tar -czvf myarchive.tar.gz file1.txt file2.txt file3.txt`  
   - **Explanation:** Creates a `.tar.gz` compressed archive  

5. 🧩 **Compress archive using `bzip2`**  
   - `tar -cjvf myarchive.tar.bz2 file1.txt file2.txt file3.txt`  
   - **Explanation:** Creates a `.tar.bz2` compressed archive, better compression  

6. ❄️ **Compress archive using `xz`**  
   - `tar -cJvf myarchive.tar.xz file1.txt file2.txt file3.txt`  
   - **Explanation:** Creates a `.tar.xz` archive, highest compression  

7. 📦 **Create a `.zip` archive**  
   - `zip myarchive.zip file1.txt file2.txt file3.txt`  
   - **Explanation:** Zip compresses and archives in one step  

8. 🗃️ **Extract files from archives**  
   - `tar -xvf myarchive.tar` → Extract `.tar`  
   - `tar -xzvf myarchive.tar.gz` → Extract `.tar.gz`  
   - `tar -xjvf myarchive.tar.bz2` → Extract `.tar.bz2`  
   - `tar -xJvf myarchive.tar.xz` → Extract `.tar.xz`  
   - `unzip myarchive.zip` → Extract `.zip`  

9. 👀 **List contents without extracting**  
   - `tar -tf myarchive.tar` → List `.tar` contents  
   - `unzip -l myarchive.zip` → List `.zip` contents  

**⚡ Tips:**  
- Practice creating, compressing, extracting, and listing archives  
- Compare different compression methods (gzip, bzip2, xz, zip)  
- Observe file sizes before and after compression to see efficiency
