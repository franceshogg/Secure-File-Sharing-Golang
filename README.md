# SECURE FILE SHARING

## Project Description

This project implements a secure file storage and sharing system in Go. Users can register with a username and password, securely store files, load them, and later append to or share those files with other users through cryptographic invitations. The system uses authenticated encryption and a secure key management scheme to maintain confidentiality, integrity, and user-level access control.

## Technologies Used

* Golang
* Git
* UUID (github.com/google/uuid)
* CS161 Userlib (github.com/cs161-staff/project2-userlib)
* JSON

## Features

List of features ready and TODOs for future development
* User account creation and authentication
* File storage and retrieval with per-user file isolation
* File appending
* Secure file sharing through invitation links
* Access revocation for previously shared files
* Usage of authenticated encryption, deterministic UUID generation, and KDFs for key security

To-do list:
* Add front-end to make project usable.

## Getting Started

- Clone the repository: git clone https://github.com/franceshogg/Secure-File-Sharing-Golang
.git
- Naviate to client-test folder:
   - cd client-test
- To test the code:
   - go test -v

## Usage

* InitUser(username, password) – Registers and initializes a new user.
* GetUser(username, password) – Authenticates and loads an existing user.
* StoreFile(filename, content) – Stores a file securely for the authenticated user.
* LoadFile(filename) – Loads the contents of a user’s file.
* AppendToFile(filename, content) – Appends to an existing file (not yet implemented).
* CreateInvitation(...) – Shares access to a file with another user (not yet implemented).
* AcceptInvitation(...) – Accepts a shared file (not yet implemented).
* RevokeAccess(...) – Revokes another user’s access to a shared file (not yet implemented).
