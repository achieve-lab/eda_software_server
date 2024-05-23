---


---

<h1 id="welcome-to-ece-eda-software-repository-for-research-purposes-only">Welcome to ECE EDA Software Repository (for Research Purposes only)</h1>
<p>Welcome to the EDA Software Repository in ECE. This repositoty houses major Electronic Design Softwares from Synopsys, Cadence, AMD-Xilinx, and Intel Altera. The key features of the repository are as follow.</p>
<ol>
<li>Hosted centrally and mountable to ECE client machines via Unix Network File System or NFS. The server is currently hosted using AlmaLinux 8.9 using NFS V4.0.</li>
<li>Central maintenance, no major additional maintenance needed in the client machine. Its a mount-and-use repository. Overall setup time is less than 5 minutes.</li>
<li><a href="https://modules.sourceforge.net/">Environment Module-based</a> no fuss setup. Portable across bash, csh, tcsh, zsh, and other commonly used shells. No maintanenace of separate .bashrc, .tchsrc, or .zshrc. Environment module allows a dynamic and plastic work environment with on-demand access of necessary tools.</li>
<li>No separate setup of Licesne strings. Transparent setup for an user.</li>
<li><a href="https://github.com/achieve-lab/eda_software_server/issues">GitHub-based</a> issue tracking for software setups.</li>
</ol>
<h3 id="how-to-mount-the-software-repository">How to Mount the software repository?</h3>
<p>Mount the software repository to your local Linux server (RHEL, CentOS, AlmaLinux, Ubuntu) using the following instructions.</p>
<pre><code>su -
mkdir -pv /EDA_Tools
vi /etc/fstab
</code></pre>
<p>Add the following line at the end of the <code>/etc/fstab</code></p>
<pre><code>eda-software-01.ece.uic.edu:/tools/EDA_Tools    /EDA_Tools          nfs defaults,_netdev    0 0
</code></pre>
<p>Then mount the NFS partition using the following command.</p>
<pre><code>mount -a
systemctl daemon-reload (only for RHEL/CentOS/AlmaLinux)
</code></pre>
<h3 id="who-can-mount-the-software-repository">Who can Mount the software repository?</h3>
<p>As of now, the repository is available on request. This is to ensure that the server is not flooded with unknown traffic. If  you like to use the repository, please send an email to Debjit Pal <a href="mailto:dpal2@uic.edu">(dpal2@uic.edu)</a>. Please include <strong>[EDA Software Server Access Request]: Lab Name</strong> in the subject line. In the email body, please provide the <strong>server IP</strong> and the <strong>server OS</strong>. After I receive your request, I will whitelist the server IP and will send you a confirmation.</p>
<h3 id="software-catalog">Software Catalog</h3>
<ul>
<li>Cadence Softwares</li>
<li>Synopsys Software</li>
<li>AMD Xilinx Softwares</li>
<li>Intel Quartus Software</li>
</ul>
<h3 id="maintained-by">Maintained by</h3>
<ul>
<li><strong>Faculty</strong>: Debjit Pal <a href="mailto:dpal2@uic.edu">(dpal2@uic.edu)</a></li>
</ul>

