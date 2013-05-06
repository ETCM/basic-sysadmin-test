Compliance Questions
====================
Answer the following immediately following the question.

Q1) Describe your experience working with regulatory compliance issues
----------------------------------------------------------------------
Restrict your answers to compliance issues such as:

- [STIGs](http://iase.disa.mil/stigs/)
- [PCI-DSS](https://www.pcisecuritystandards.org/security_standards/index.php)
- [SOX](http://www.gpo.gov/fdsys/pkg/BILLS-107hr3763enr/html/BILLS-107hr3763enr.htm)


This list is suggestive, not restrictive. Include details pertaining to system
configuration, auditing and verification.

PCI-DSS
I have contracted for a couple of companies that are not currently PCI compliant but hope to obtain this distinction. In doing so I have participated in project that segment non-authorized systems from accessing restricted resources such as credit cards and PII. Doing so included creating VLAN and segmenting the networks off from each other in order to keep within strict budget constraints. Implementation of firewalls with quasi-DLP functionality have also been attempted to prevent credit card information and personal information such as social security numbers from leaving the network.

These environments have also been non-formally assessed to see what vulnerabilities and risk exist. The primary goal of these assessments were to bring these issues to the attention of the leadership within these companies. 

HIPAA
Two of the clients I have supported deal with HIPAA compliance. I have been involved in implementing systems that must be protected from invalid access. I have also had to educate users on what they proper and improper procedures were when asked for assistance. Configuration of firewalls and other network security devices also occurred as well as being involved in the processes of ensuring that proper backup procedures were being followed.  

Q2) Broadly describe how you would investigate the following scenario:
----------------------------------------------------------------------
You have a public facing site running PHP 5.4.12, Apache 2.2.24, MySQL 5.5.30
and vBulletin 4.2.0. The provisioning record does not mention what kernel is
installed, but the machine is a Linux host. The site runs custom software
providing an electronic store for a niche good and hosts an enthusiast
discussion community.

The forum moderators report the existence of a post mocking the site
administrators for an inability to secure data. A fragment of the owner's
private profile information is in the post.

Bullet points will suffice for this.

- Create bit level copy of the system
- Verify if any data is actually insecure
- Copy all log data such as Apache Access Logs and MySQL logs
- Set up monitoring for the particular user within reason
- Update all software to the current versions and patch levels



Q3) Describe how distributions like RHEL complicate compliance issues.
----------------------------------------------------------------------
The only complications I can see is that these distributions may need to be tailored to comply with different types compliances and their rules. It may not support all requirements that a particular compliance expects.
