### Data Flow Diagram Dictionary

# Databases
* OSS License Compliance Database: Database 
* NIST CPE Info: Is the database where CPE Information is stored, it is a global database.
* OSS Database
* Policy Database

#External Entities
* Online Repository:
* Corporate Developer: An employee in the IT department who is responsible for managing code stream.
* Corporate Manager: An employee in the IT department who manages information regarding project.
* National Vulnerability Database: Vulnarabitity details of software are stored, and CPE/CVE information is obtained from this database.

#Processes
* Send Flagged Code to Online Repository: This process will send flagged code back to the community.
* Version Control:
* Manage Code Streams :A process in which files and packages are scanned for license information, CPE/CVE information and then the information is retreived from the OSS database when required.
* Manage CPE Information:A process in which CPE request is sent to the National Vulnaribity Dataase and the received information is stored in NIST CPE Datastore.

#Data Flows
* File/Package: A single file or a collection of files in a package.
* CVE Information :It is the information used to find vulnarabilities in packages.
* License Scanner: Used to find copy left, copy right and other licenses in packages
