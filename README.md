# tilted-rails

A sandbox for playing with Tilt extensions that generate and deploy a new Rails/Postgres application to Kubernetes.

To try it, check out this repository and run `tilt up` in it. The first time it runs, a database and a plain pod with Rails installed get deployed under the `extensions.rails-db` and `extensions.rails` labels, and a new Rails app is generated inside the pod with Rails, then copied to your local disk. Tilt will then build an image for the Rails app, deploy it to K8, and port-forward localhost:3000.
