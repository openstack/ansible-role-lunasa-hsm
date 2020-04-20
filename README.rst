lunasa-hsm
==========

A role to manage Safenet Lunasa Hardware Security Module (HSM) client software.

Role Variables
--------------

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
   * - lunasa_hsm_server_hostname
     - None
     - Hostnme for the Lunasa HSM.
   * - lunasa_hsm_server_admin_password
     - None
     - Password for the admin user for the Lunasa HSM.
   * - lunasa_hsm_partition
     - None
     - HSM Partition to assign the client.
   * - lunasa_client_ip
     - None
     - IP to use when registering the client.

Requirements
------------

 - ansible >= 2.4
