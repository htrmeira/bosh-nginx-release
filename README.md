# bosh-nginx-release
Simple BOSH release for nginx.

The purpose of this is to learn hoe to create and deploy a BOSH release. It is derived from the Anynines [homework](https://github.com/anynines/homework).

An example manifest to deploy this release can be found under the examples/ directory.

Steps:
- First add the blobs to the blobstore with: bosh add blob <tgz_path> nginx

Then,
Setup the deployment manifest: bosh deployment examples/manifest-openstack.yml

bosh create release

bosh upload release

bosh deploy

Make sure you are using the correct manifest file
