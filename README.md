# Active Directory Home Lab

I built this lab to practise Windows administration and common IT support tasks.

## Lab setup

| Machine | Operating system | Purpose |
|---|---|---|
| LAB-DC01 | Windows Server 2025 | Active Directory, DNS and shared folder |
| LAB-PC01 | Windows 11 Enterprise | Domain workstation |

- **Platform:** VirtualBox
- **Domain:** itlab.test
- **Server IP:** 192.168.50.10
- **Network:** VirtualBox NAT Network

## What I completed

- Installed Active Directory and DNS.
- Joined a Windows 11 computer to the domain.
- Created users, security groups and organisational units.
- Applied a Group Policy showing a sign-in message.
- Created a shared folder with group-based permissions.
- Reset a user's password and required a password change.

## Tests and results

| Test | Result |
|---|---|
| Sign in as a domain user | Successful |
| Display the Group Policy sign-in message | Successful |
| Access the Staff share as Alex | Allowed |
| Access the share as Jamie without group membership | Denied |
| Add Jamie to GG_Staff and sign in again | Access allowed |
| Reset Jamie's password and change it at sign-in | Successful |

## Troubleshooting

### Windows 11 black screen
Changing the client VM from two to three virtual CPUs resolved the startup problem in my lab.

### DNS timeout
The domain controller was switched off. Starting it restored domain DNS responses.

## Skills practised

Active Directory, DNS, Group Policy, Windows administration,
shared-folder permissions, user management and troubleshooting.

## Screenshots

Screenshots will be added to show the setup and test results.

## Notes

This is a personal training lab using fictional users and evaluation
software. Passwords and virtual machine files are not included.
