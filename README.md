# Distributed File Storage and Retrieval System
This project implements a Distributed File Storage and Retrieval System using Python. It consists of a Directory Server, multiple Node Servers, and a Client application. The Directory Server manages the registry of Node Servers and tracks the location of stored files. Node Servers are responsible for storing and retrieving files, and the Client is used to upload and download files to/from Node Servers.

File Structure
plaintext
Copy code
DistributedFileStorageSystem/
│
├── DirectoryServer/
│   ├── directory_server.py  # Directory Server implementation
│   └── requirements.txt     # Required Python packages
│
├── NodeServer/
│   ├── node_server.py       # Node Server implementation
│   ├── storage/             # Directory for storing files
│   └── requirements.txt     # Required Python packages
│
└── Client/
    ├── client.py            # Client application
    └── requirements.txt     # Required Python packages
Setup and Installation
Directory Server
Navigate to the DirectoryServer directory.
Install the required packages:
Copy code
pip install -r requirements.txt
Run the Directory Server:
Copy code
python directory_server.py
Node Server
Navigate to the NodeServer directory.
Install the required packages:
Copy code
pip install -r requirements.txt
Run the Node Server:
Copy code
python node_server.py
Client
Navigate to the Client directory.
Install the required packages:
Copy code
pip install -r requirements.txt
Use client.py to upload or download files.
Usage
Uploading a File
To upload a file, use the upload_file method in the client.py script:

python
Copy code
client.upload_file('path/to/file.txt')
Downloading a File
To download a file, use the download_file method, specifying the file ID and the download location:

python
Copy code
client.download_file('file.txt', 'path/to/download')
Additional Files
requirements.txt: Each component should have its own requirements.txt file listing the necessary Python packages. For this project, the primary dependency is the Python socket library, which is part of the standard library.
Contributing
Contributions to this project are welcome. Please ensure to follow best practices for code style and commit messages.
