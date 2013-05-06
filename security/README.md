Security
========

Q1) What is SSL?
----------------
Secure Sockets Layer is a cryptographic protocol that allows for secure transmission of data across unsecured networks. The primary goals of this protocol are to provide cryptographic security and interoperability between applications.

Q2) What is the sudoers file? What is its purpose?
--------------------------------------------------
The sudoers file is a linux module that defines sudo permission for users and groups within a system. When a sudo command is issued by a user the sudoers file is used to determine what actions can be taken in this elevated state.

Q3) Compare and contrast password, key and certificate authentication.
----------------------------------------------------------------------
Password, key and certificate are all methods that can be used to authenticate to particular resources. The all work by presenting a credential to an authentication authority so that resources can be reached. The process in which the authentication is achieved differs for each of the three types.

Password authentication is the most basic and one of the most commonly used authentication techniques. A client must present the correct set of credentials to the authentication authority in order to be granted access or rights to resources. The authentication authority has access to the proper password and checks the client password against the one that it has stored. If the are correct then the client is authenticated. Passwords can become less effective when users are entered in to the equation. 

Key authentication employs encryption keys to authenticate a client. Public or private key techniques can be used to achieve authentication. A public/private key pair can be used. The private key is used to encrypt a message which is then sent to the authentication authority. The authentication authority then uses the public key to decrypt the message. If decryption is successful then the client is authenticated. This method can also be used for widespread authentication so that multiple parties can verify the identity of the sending party. Private key cryptography can also be used but is less scalable. The same key used to encrypt the message must be used to decrypt it. This method can be automated so that users are removed from management.

Certificate authentication uses a public key to sign a certificate. Certificates use the PKI infrastructure to validate that a certificate and verify identity. A client can present a ticket to an authentication authority and that authority will use a certificate authority to verify the authenticity of the certificate. It also can check against the certificate authority's revocation list to make sure that the certificate hasn't been revoked or compromised. This trust structure allows for authentication by a third trusted party. This method of authentication can be managed my software so that users are removed from the equation.

Q4) How do you enable certificate authentication in Apache?
-----------------------------------------------------------
1 Create a Java Key Store that has the self-signed certificate you will be using
2 Modify the server.xml file to have parameters matching the parameters of the Java Key Store
3 Create a Certificate Authority and an associated Java Key Store for the CA
4 Modify the server.xml file so that the truststoreFile attribute is associated with the CA that was created. Change the clientAuth attribute to true to enable the feature.


Q5) How do you handle a leaked key?
-----------------------------------
If a key is compromised it should be removed from production. It also needs to be submitted for revocation so that all parties know the key should no longer be used and is potentially a liability. The revoked key should then be placed in a safe location and new keys should be generated.
