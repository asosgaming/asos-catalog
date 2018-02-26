<!-- BEGIN MUNGE: UNVERSIONED_WARNING -->


<!-- END MUNGE: UNVERSIONED_WARNING -->

# Persistent Installation of MySQL and WordPress on Rancher

## Visit your new WordPress blog

To access your new installation, you first may need to open up port 80 (the port specified in the wordpress service config) in the firewall for your cluster. You can do this, e.g. via:

This will define a firewall rule called `sample-http` that opens port 80 in the default network for your project.

Now, we can visit the running WordPress app.
Use the external IP that you obtained above, and visit it on port 80:

```
http://<external-ip>
```

You should see the familiar WordPress init page.


If you want to shut down the entire app installation, you can delete the services as well.

If you are ready to turn down your Kubernetes cluster altogether, run:

```sh
$ cluster/kube-down.sh
```




<!-- BEGIN MUNGE: IS_VERSIONED -->
<!-- TAG IS_VERSIONED -->
<!-- END MUNGE: IS_VERSIONED -->
