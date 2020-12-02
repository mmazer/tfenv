### tfenv

Simple shell scripts to manage and run different Terraform versions. Inspired by [rbenv](https://github.com/rbenv/rbenv) but kept as simple as possible:

 - set a default, global Terraform version
 - set a shell environment specific version

#### Installation

```
git clone https://github.com/mmazer/tfenv.git ~/.tfenv
```

Update your shell's `PATH` to include `~/.tfenv/bin` or run `eval "$(~/.tfenv/bin/tfenv -i)`.

#### Installing Terraform

Download [Terraform](https://www.terraform.io/downloads.html) and copy the files into `~/.local/share/tfenv/versions`. Ensure the filename includes the Terraform version, e.g `terraform-0.12.28`.

#### Running tfenv

Set a global version after installing a terraform version:

```
$ tfenv -g 0.12.28
$ # run Terraform wrapper ~/.tfenv/bin/terraform
$ terraform version
Terraform v0.12.28
```

