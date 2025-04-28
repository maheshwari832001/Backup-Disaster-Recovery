# TITLE:  Backup and Disaster Recovery Using Windows 10 and OpenMediaVault NAS

## Objective
The objective of this project is to design a practical Backup and Disaster Recovery mechanism. It involves protecting important files from Windows 10 by backing them up onto OpenMediaVault NAS storage and ensuring successful restoration after data loss events, showcasing real-world disaster recovery strategies.

## Tools Used
- Windows 10 (Host System)
- Oracle VirtualBox (Virtualization Platform)
- OpenMediaVault NAS Server (running in VirtualBox)
- SMB/CIFS (Network File Sharing Protocol)

##  Setup Steps:
1. **Prepared OpenMediaVault NAS:**
   - Created a shared folder named `BackupStorage`.
   - Enabled and configured SMB/CIFS sharing.
   - Set permissions for access.

2. **Connected Windows 10 to OMV:**
   - Map `BackupStorage` shared folder as a network drive (Z:).

3. **Performed Backup:**
   - Created a folder `ImportantData` with various file types.
   - Copied `ImportantData` to BackupStorage (Z:).

4. **Simulated Disaster:**
   - Deleted `ImportantData` from Windows system.

5. **Recovery:**
   - Restored the deleted `ImportantData` by copying it back from BackupStorage.

## Conclusion
This project successfully demonstrated how to set up a backup system using NAS storage, simulate a disaster event, and recover lost data effectively, emphasizing the importance of structured backup and disaster recovery strategies.

