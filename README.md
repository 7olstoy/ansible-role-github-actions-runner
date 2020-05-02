# github-actions-runner-ansible-role
Very tiny and easy ansible role for fast ADD and REMOVE github actions runner

Example use:
```
- name: Get GitHub runner
  hosts: server
  vars:
    runner_mode: "install" # or uninstall
    runner_version: "2.169.1"
    runner_user: "user"
    runner_name: "user"
    runner_dir: "/home/user/actions-runner"
    github_repo: "https://github.com/user/repo"
    github_repo_name: "user-repo"
    github_token: "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
  roles:
    - github-actions-runner-ansible-role
```

Please note: *github_token* valid only for one install and uninstall, after that you need to change it.
