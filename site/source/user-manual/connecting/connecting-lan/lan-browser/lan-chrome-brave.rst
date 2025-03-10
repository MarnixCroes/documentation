.. _lan-chrome-brave:

=================================================
Trusting Your Start9 CA in Chrome / Brave Browser
=================================================

.. caution:: You will first need to complete :ref:`lan-os` for your device before continuing.

.. note:: This guide will work for Chrome, Chromium, Brave Browser or Vivaldi

.. tabs::

    .. group-tab:: Linux

        #. Open a new tab in the browser and open to "Settings" from the top-right hamburger menu.

            .. figure:: /_static/images/ssl/browser/brave_settings.png
              :width: 30%
              :alt: Chrome / Brave settings page

        #. On the left hand sidebar, select the "Privacy and security" section, then the "Security" menu item.

            .. figure:: /_static/images/ssl/browser/brave_security.png
              :width: 60%
              :alt: Chrome / Brave Privacy and security settings

        #. At the bottom of the section, select "Manage Certificates".
        
            .. figure:: /_static/images/ssl/browser/brave_security_settings.png
              :width: 60%
              :alt: Chrome / Brave Security settings page

        #. Click the "Authorities" tab

            .. figure:: /_static/images/ssl/browser/brave-authorities.png
              :width: 60%
              :alt: Certificate Authorities

        #. If you see "org-Start9" with a trusted “<custom-address> Local Root CA” listed under it, your work is already done. Open a new tab and visit your Start9 server's ``.local`` address.  The browser shouldn't give any warning pages about the certificate anymore.  If it still does, quit and restart the browser using `Menu > Exit`.

        #. If you do not see "org-Start9" in the list, click "Import" and open the downloaded "<custom-address> Local Root CA.crt" file on your device.
        
            .. figure:: /_static/images/ssl/browser/chrome_authorities.png
              :width: 60%
              :alt: Chrome / Brave Import "<custom-address>.crt"

        #. Check the box for "Trust this certificate for identifying websites" and click "OK".

            .. figure:: /_static/images/ssl/browser/chrome_trust.png
              :width: 60%
              :alt: Chrome / Brave Manage Certificates sub-menu on macOS


    .. group-tab:: Windows

        #. Open a new tab in the browser and click "Settings" from the top-right hamburger menu.

            .. figure:: /_static/images/ssl/browser/brave_settings.png
              :width: 30%
              :alt: Brave settings page

        #. On the left hand sidebar, select the "Privacy and security" section, then the "Security" menu item.

            .. figure:: /_static/images/ssl/browser/brave_security.png
              :width: 60%
              :alt: Brave Privacy and security settings

        #. At the bottom of the section, select "Manage Certificates".
        
            .. figure:: /_static/images/ssl/browser/brave_security_settings.png
              :width: 60%
              :alt: Brave Security settings page

        #. The Windows Certificates Manager will open.  Click the `Trusted Root Certification Authorities` tab, then `Import...`

            .. figure:: /_static/images/ssl/windows/windows_certificates_caimport_step1.jpg
              :width: 40%
              :alt: Windows Certificates CA Cert Import Step 1

        #. The Windows Certificate Import Wizard will open.  Click `Next`

            .. figure:: /_static/images/ssl/windows/windows_certificates_caimport_step2.jpg
              :width: 40%
              :alt: Windows Certificates CA Cert Import Step 2

        #. Click `Browse...` to select the CA Cert

            .. figure:: /_static/images/ssl/windows/windows_certificates_caimport_step3.jpg
              :width: 40%
              :alt: Windows Certificates CA Cert Import Step 3

        #. Navigate to the location of and select your previously downloaded `<custom-address>.crt` file, and click `Open`

            .. figure:: /_static/images/ssl/windows/windows_certificates_caimport_step4.jpg
              :width: 40%
              :alt: Windows Certificates CA Cert Import Step 4

        #. The path to the CA certificate will be filled in.  Click `Next`

            .. figure:: /_static/images/ssl/windows/windows_certificates_caimport_step5.jpg
              :width: 40%
              :alt: Windows Certificates CA Cert Import Step 5

        #. Ensure `Place all certificates in the following store` is selected and the Certificate store is set to `Trusted Root Certification Authorities`.  Click `Next`

            .. figure:: /_static/images/ssl/windows/windows_certificates_caimport_step6.jpg
              :width: 40%
              :alt: Windows Certificates CA Cert Import Step 6

        #. Click `Finish`

            .. figure:: /_static/images/ssl/windows/windows_certificates_caimport_step7.jpg
              :width: 40%
              :alt: Windows Certificates CA Cert Import Step 7

        #. Click `Yes` to accept the subsequent Security Warning

            .. figure:: /_static/images/ssl/windows/windows_certificates_caimport_step8.jpg
              :width: 40%
              :alt: Windows Certificates CA Cert Import Step 8

        #. The Windows Certificates Manager should report that the certificate import was successful.  Click `OK`, then `Close`

            .. figure:: /_static/images/ssl/windows/windows_certificates_caimport_step9.jpg
              :width: 40%
              :alt: Windows Certificates CA Cert Import Step 9

    .. group-tab:: Mac

       No additional setup is required for Chrome or Brave on MacOS