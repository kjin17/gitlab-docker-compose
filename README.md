# Gitlab initial Password

    root@gitlab:/# cd /etc/gitlab/
    root@gitlab:/etc/gitlab# ls
    gitlab-secrets.json  initial_root_password  ssh_host_ecdsa_key.pub  ssh_host_ed25519_key.pub  ssh_host_rsa_key.pub
    gitlab.rb            ssh_host_ecdsa_key     ssh_host_ed25519_key    ssh_host_rsa_key          trusted-certs
    root@gitlab:/etc/gitlab# cat initial_root_password 

    # WARNING: This value is valid only in the following conditions

    #          1. If provided manually (either via `GITLAB_ROOT_PASSWORD` environment variable or via `gitlab_rails['initial_root_password']` setting in 
    `gitlab.rb`, it was provided before database was seeded for the first time (usually, the first reconfigure run).

    #          2. Password hasn't been changed manually, either via UI or via command line.

    #

    #          If the password shown here doesn't work, you must reset the admin password following https://docs.gitlab.com/ee/security
    /reset_user_password.html#reset-your-root-password.


    Password: OnKalyBRomxQEWGYgfKQwCox/UNx/Y0WPK/ae/jUloM=


    # NOTE: This file will be automatically deleted in the first reconfigure run after 24 hours.
