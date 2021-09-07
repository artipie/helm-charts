# helm-charts
Helm charts with Artipie

## Usage

To install Artipie into k8s cluster you need:
 1. Get dependencies: run `helm build ./artipie`
 2. Install chart: run `helm install artipie ./artipie`

On install, you need to specify correct service type for `artipie` via
`service.type` value, e.g. `helm install --set service.type=NodePort artipie ./artipie`.

After installation you can access Artipie via `artipie` service.

## Configuration

TBD

## Details

Cluster setup uses `etcd` as configuration storage.
