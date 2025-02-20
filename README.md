# cloudmux

## Command line tool

### Complile

```bash
$ make cmd/cmx
```

### Example

1. List regions

```bash
# Aliyun
$ ./_output/bin/cmx --provider Aliyun  --access-key $your_access_key --secret $your_secret region-list 

# Aws
$ ./_output/bin/cmx --provider Aws --cloud-env ChinaCloud  --access-key $your_access_key --secret $your_secret --debug region-list

# Azure
$ ./_output/bin/cmx --provider Azure --cloud-env AzurePublicCloud \
    --access-key $your_directory_id/$your_subscription_id \
    --secret $your_app_id/$your_app_key \
    region-list
```

2. List zones

```bash
# Aliyun
$ ./_output/bin/cmx --provider Aliyun  --access-key $your_access_key --secret $your_secret zone-list
```

3. List VM instances

```bash
# Aliyun
$ ./_output/bin/cmx --provider Aliyun --region ap-southeast-1 --access-key $your_access_key  --secret $your_secret  instance-list --zone ap-southeast-1a
```
