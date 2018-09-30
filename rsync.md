<!-- TITLE: Rsync -->
<!-- SUBTITLE: A quick summary of Rsync -->

# Header
Here's an example of a command I would use to sync files from Linode B to Linode A:

    $ rsync -avziP  ~/local_directory_path username@remote_host_IP:/destination_directory

A few important notes regarding rsync, is that you should turn off as many services as possible while the data is syncing. Also, you should test your command on a test directory before syncing the whole server to make sure it is working as expected.

Copying Files Locally:

   $ rsync -avziP  /dev/linode-disk /dev/block-storage-volume