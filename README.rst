lunasa-hsm
==========

A role to manage Thales Luna Network Hardware Security Module (HSM) clients.

Role Variables
--------------

This ansible role automates the configuration of a new client for the
Thales Luna Network HSM.

.. list-table::
   :widths: auto
   :header-rows: 1

   * - Name
     - Default Value
     - Description
   * - lunasa_client_working_dir
     - /tmp/lunasa_client_install
     - Working directory in the target host.
   * - lunasa_client_tarball_name
     - None
     - Filename for the Lunasa client software tarball.
   * - lunasa_client_tarball_location
     - None
     - Full URL where a copy of the client software tarball can be downloaded.
   * - lunasa_client_installer_path
     - None
     - Path to the instal.sh script inside the tarball.
   * - lunasa_client_pin
     - None
     - The HSM Partition Password (PKCS#11 PIN) to be used by the client.
   * - lunasa_client_ip
     - None
     - (Optional) When set, this role will use the given IP to register
       the client instead of the client's fqdn.
   * - lunasa_client_rotate_cert
     - False
     - When set to True, the role will generate a new client certificate
       to replace the previous one.
   * - lunasa_hsms
     - None
     - List of dictionaries, each of which describes a single HSM
       `see vars.sample.yaml` for details.  When more than one HSM is
       listed here, the client will be configured in HA mode.

Requirements
------------

 - ansible >= 2.4
