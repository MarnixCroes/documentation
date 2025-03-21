.. _backup:

======
Backup
======

.. contents::
  :depth: 2 
  :local:

Backing up your server is easy and secure. Backups are encrypted with your master password.

.. warning:: Create frequent backups to avoid loss of data!

Setup Device
------------

Select your platform for detailed instructions on how to create a Network Folder for creating backups (recommended).  Otherwise, you may backup to a physical drive, attached in addition to your main server's SSD.

.. toctree::
  :maxdepth: 1

  Linux Network Folder <backup-setup/backup-linux>
  Mac Network Folder <backup-setup/backup-mac>
  Windows Network Folder <backup-setup/backup-windows>
  Synology Network Folder <backup-setup/backup-synology>
  TrueNAS Network Folder <backup-setup/backup-truenas>
  Physical Drive <backup-setup/backup-physical>

.. _backup-create:

Create Backup
-------------

#. Go to *System > Create Backup*

    .. figure:: /_static/images/config/backup.png
        :width: 60%

#. You will see your previously created Network Folder backup location (or Physical Drive) available.  Click it, then click "Create Backup".

    .. figure:: /_static/images/config/backup2.png
        :width: 60%

#. You can continue to use your server while the backup is in progress.

    .. figure:: /_static/images/config/backup3.png
        :width: 60%

#. When the backup is complete, you will receive a notification.  If successful, you will see the date and time of your most recent backup updated under "Backups" in the System tab.

    .. figure:: /_static/images/config/backup4.png
        :width: 60%
