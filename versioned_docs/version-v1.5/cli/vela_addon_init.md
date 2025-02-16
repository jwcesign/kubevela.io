---
title: vela addon init
---

create an addon scaffold

### Synopsis

Create an addon scaffold for quick starting.

```
vela addon init [flags]
```

### Examples

```
  Store the scaffold in a different directory:
	vela addon init mongodb -p path/to/addon

  Add a Helm component:
	vela addon init mongodb --helm-repo https://marketplace.azurecr.io/helm/v1/repo --chart mongodb --chart-version 12.1.16

  Add resources from URL using ref-objects component
	vela addon init my-addon --url https://domain.com/resource.yaml

  Use --no-samples options to skip creating sample files
	vela addon init my-addon --no-sample

  You can combine all the options together.
```

### Options

```
      --chart string           Helm Chart name
      --chart-version string   version of the Chart
  -f, --force                  overwrite existing addon files
      --helm-repo string       URL that points to a Helm repo
  -h, --help                   help for init
      --no-samples             do not generate sample files
  -p, --path string            path to the addon directory (default is ./<addon-name>)
  -u, --url stringArray        add URL resources using ref-object component
```

### Options inherited from parent commands

```
  -y, --yes   Assume yes for all user prompts
```

### SEE ALSO

* [vela addon](vela_addon)	 - Manage addons for extension.

#### Go Back to [CLI Commands](vela) Homepage.


###### Auto generated by [spf13/cobra script in KubeVela](https://github.com/kubevela/kubevela/tree/master/hack/docgen).
