# terraform-github-repository
Terraform module which creates GitHub repository resources.

<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_github"></a> [github](#requirement\_github) | 5.41.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_github"></a> [github](#provider\_github) | 5.41.0 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [github_branch_protection.self](https://registry.terraform.io/providers/integrations/github/5.41.0/docs/resources/branch_protection) | resource |
| [github_repository.self](https://registry.terraform.io/providers/integrations/github/5.41.0/docs/resources/repository) | resource |
| [github_team_repository.self](https://registry.terraform.io/providers/integrations/github/5.41.0/docs/resources/team_repository) | resource |
| [github_team.self](https://registry.terraform.io/providers/integrations/github/5.41.0/docs/data-sources/team) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_allow_auto_merge"></a> [allow\_auto\_merge](#input\_allow\_auto\_merge) | Whether to allow auto-merging pull requests | `bool` | `false` | no |
| <a name="input_allow_merge_commit"></a> [allow\_merge\_commit](#input\_allow\_merge\_commit) | Whether to allow merge commits | `bool` | `false` | no |
| <a name="input_allow_rebase_merge"></a> [allow\_rebase\_merge](#input\_allow\_rebase\_merge) | Whether to allow rebase merges | `bool` | `true` | no |
| <a name="input_allow_squash_merge"></a> [allow\_squash\_merge](#input\_allow\_squash\_merge) | Whether to allow squash merges | `bool` | `true` | no |
| <a name="input_description"></a> [description](#input\_description) | The description of the repository | `string` | n/a | yes |
| <a name="input_gitignore_template"></a> [gitignore\_template](#input\_gitignore\_template) | The gitignore template of the repository | `string` | `null` | no |
| <a name="input_has_branch_protection"></a> [has\_branch\_protection](#input\_has\_branch\_protection) | Whether the repository has branch protection enabled | `bool` | `true` | no |
| <a name="input_has_discussions"></a> [has\_discussions](#input\_has\_discussions) | Whether the repository has discussions enabled | `bool` | `false` | no |
| <a name="input_has_issues"></a> [has\_issues](#input\_has\_issues) | Whether the repository has issues enabled | `bool` | `false` | no |
| <a name="input_has_projects"></a> [has\_projects](#input\_has\_projects) | Whether the repository has projects enabled | `bool` | `false` | no |
| <a name="input_has_wiki"></a> [has\_wiki](#input\_has\_wiki) | Whether the repository has wiki enabled | `bool` | `false` | no |
| <a name="input_license_template"></a> [license\_template](#input\_license\_template) | Wheter the repository uses a license template | `string` | `null` | no |
| <a name="input_name"></a> [name](#input\_name) | The name of the repository | `string` | n/a | yes |
| <a name="input_owner"></a> [owner](#input\_owner) | The name of the repository | `string` | n/a | yes |
| <a name="input_required_status_checks_contexts"></a> [required\_status\_checks\_contexts](#input\_required\_status\_checks\_contexts) | The list of status checks to require in order to merge into this branch | `list(string)` | `[]` | no |
| <a name="input_teams"></a> [teams](#input\_teams) | The teams to grant access to, and their permission levels | `map(string)` | `{}` | no |
| <a name="input_topics"></a> [topics](#input\_topics) | The topics of the repository | `list(string)` | `[]` | no |
| <a name="input_visibility"></a> [visibility](#input\_visibility) | The visibility of the repository | `string` | `"private"` | no |
| <a name="input_vulnerability_alerts"></a> [vulnerability\_alerts](#input\_vulnerability\_alerts) | Whether the repository has vulnerability alerts enabled | `bool` | `false` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_full_name"></a> [full\_name](#output\_full\_name) | The full name of the repository. |
| <a name="output_git_clone_url"></a> [git\_clone\_url](#output\_git\_clone\_url) | The Git URL of the repository. |
| <a name="output_html_url"></a> [html\_url](#output\_html\_url) | The HTML URL of the repository. |
| <a name="output_http_clone_url"></a> [http\_clone\_url](#output\_http\_clone\_url) | The HTTP URL of the repository. |
| <a name="output_node_id"></a> [node\_id](#output\_node\_id) | The Node ID of the repository. |
| <a name="output_repo_id"></a> [repo\_id](#output\_repo\_id) | The ID of the repository. |
| <a name="output_ssh_clone_url"></a> [ssh\_clone\_url](#output\_ssh\_clone\_url) | The SSH URL of the repository. |
| <a name="output_svn_url"></a> [svn\_url](#output\_svn\_url) | The SVN URL of the repository. |
<!-- END_TF_DOCS -->
