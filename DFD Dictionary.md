### Data Flow Diagram Dictionary

# Databases
* OSS License Compliance Database: Database where the licenses and copyleft information is stored.
* NIST CPE Info: Is the database where CPE Information is stored, it is a global database.
* OSS Database: The database where all of the information about the project is stored.
* Policy Database: Database that holds all the company's policy information for the project.

#External Entities
* Online Repository: This entitiy represents the open source repositories where code is taken and returned after use according to copyleft licensing.
* Corporate Developer: An employee in the IT department who is responsible for managing code stream.
* Corporate Manager: An employee in the IT department who manages information regarding project.
* National Vulnerability Database: Vulnarabitity details of software are stored, and CPE/CVE information is obtained from this global database.

#Processes
* Send Flagged Code to Online Repository: This process will send flagged code back to the community.
* Version Control: Process which allows the developer to check in and manage code.
* Manage Code Streams : A process in which files and packages are scanned for license information, CPE/CVE information and then the information is retreived from the OSS database when required.
* Manage CPE Information: A process in which CPE request is sent to the National Vulnaribity Dataase and the received information is stored in NIST CPE Datastore.
* License Scanner: This process provides scans packages or files for license information.  
* CVE Lookup: This process uses CPE information to query the National Vulnerability Database for CVE information.
* Manage Policy Information: This process takes information about the OSS and checks to see if there is a match within the company's policies.
* Manage Proejct Information: This process provides the Corporate Manager with file/package information about the project.

#Data Flows
* File/Package: A single file or a collection of files in a package.
* Project File: A single file containing code.
* License Information: Information returned about the licenses within the file/package.
* CPE Information: Contains all CPE information from the National Vulnerability Database.
* Package Name: The name of the package that is/was submitted by the developer.
* CVE Information :It is the information used to find vulnerabilities in packages.
* File SHA1 Request: A request, using a hash to see if a file already exists in the database.
* File SHA1 Response: A "yes" or "no" response from the database to confirm or deny the presence of the file in the database.
* File License, CPE, and CVE Information: 
* File Information Request: Request sent from the corporate manager to the OSS database for all relevant information in relation to the project.
* File Information Response: Response sent to the corporate manager including all relevant information about the file.
* Project Information Request: Request sent by the corporate manager for project information from the OSS database.
* Project Information Response: Response sent back to the corporate manager about project information.
* Project Policy Request: Corporate manager requests policy information related to the project.
* Project Policy Response: Policy information about the project is returned to the manager.
* Project Information Request: The policy database is queried for policy information for the project.
* Project Information Response: The policy information for the specific project is returned.
* CPE Request: A request for updated CPE information from the National Vulnerability Database.
* CPE Response: Updated CPE information is returned.
* CVE Request: Information about the CVE of a file/package is requested from the National Vulnerability Database using CPE information.
