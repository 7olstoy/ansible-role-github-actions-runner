# ansible-role-github-actions-runner

Very tiny and easy ansible role for fast ADD and REMOVE github actions runner

Example use:
```
- name: Get GitHub runner
  hosts: server
  vars:
    runner_mode: "install" # or uninstall
    runner_version: "2.277.1"
    runner_user: "user"
    runner_name: "user"
    runner_dir: "/home/user/actions-runner"
    github_repo: "https://github.com/user/repo"
    github_repo_name: "user-repo" # All / convert to -
    github_token: "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
  roles:
    - ansible-role-github-actions-runner

```

Please note: *github_token* valid only for one install and uninstall, after that you need to change it.
