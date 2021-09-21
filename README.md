👹 JONKERS 👹

Manages the deployment and observation of multi-service K8s projects

## fend

A React-based UI for managing K8s projects.

## bend

An ExpressJS-based https webserver to act as an API and serve `fend`.

## TODO

Some manner of declarative self-deployment manifest.
Jonkers will require a backing datastore (probably MongoDB), and potentially
more in the future - perhaps each service (fend, bend, datastore, etc.) should
have its own folder w/ container information etc., and then there should be a top
level manifest for orchestrating the services - and acting as deployment
instructions? I suppose if the datastore is nothing but a MongoDB image, then
the folder can be skipped and the manifest can just reference the desired image.
