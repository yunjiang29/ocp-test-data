# ocp-test-data

## Bastion host
We use Fedora coreos os as our bastion host in pipeline, `coreos-for-bastion-host/images.json` was copied from `https://builds.coreos.fedoraproject.org/streams/stable.json`, and added images for non-public regions (AWS GovCloud and AWS China images), these private images were created from https://builds.coreos.fedoraproject.org/prod/streams/stable/builds/34.20210821.3.0/x86_64/fedora-coreos-34.20210821.3.0-aws.x86_64.vmdk.xz

## Coreos in non-public regions
coreos is not published on non-public regions, like AWS GovCloud, AWS China, installing OCP on these region, a custom AMIs must be provided.
CI pipelines could get pre-created AMIs for non-public regions from `coreos-for-non-public-regions/images.json`
