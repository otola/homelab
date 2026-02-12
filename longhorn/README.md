# Longhorn Deployment Notes

* Once deployed the default storageclass of local-path should be set to false by editing the existing annotation.
* The current set up is hosted on a single node host, therefore the defaultReplicaCount is set to 1 and autoSalvage is set to false. These will need to be updated once additional hosts are added to the cluster.
* Volume backups are configured to use CIFS,  the referenced secret will need to be created beforehand.
