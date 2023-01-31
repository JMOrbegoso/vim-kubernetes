# vim-kubernetes

Forked from [andrewstuart/vim-kubernetes](https://github.com/andrewstuart/vim-kubernetes).

This package provides kubernetes YAML snippets (requires [ultisnips](https://github.com/sirver/UltiSnips), as well as a number of integrations with kubectl (requires that you actually have kubectl installed and on your `PATH`).

## Installation

Vim-Plug:

```vim
Plug 'JMOrbegoso/vim-kubernetes'
```

Vundle:

```vim
Plugin 'JMOrbegoso/vim-kubernetes'
```

## Functions/Commands

For the current buffer (including modifications not saved on disk)

- `:KubeApply`
- `:KubeDelete`
- `:KubeCreate`

And for the current directory (read from disk)

- `:KubeApplyDir`
- `:KubeDeleteDir`

If you would like to bind any of these to a shortcut, you can do something like
the following in your `~/.vimrc`:

```vim
au FileType yaml nmap <leader>r :KubeApply<CR>
```

## Snippets

| Resource                        | snippet   |
| ------------------------------- | --------- |
| Cert-Manager Certificate        | cert      |
| ConfigMap                       | cm        |
| DaemonSet                       | ds        |
| Deployment                      | deploy    |
| HorizontalPodAutoscaler v1      | hpa1      |
| HorizontalPodAutoscaler v2      | hpa2      |
| HorizontalPodAutoscaler v2beta1 | hpa2beta1 |
| HorizontalPodAutoscaler v2beta2 | hpa2beta2 |
| Ingress                         | ing       |
| Kubernetes Cronjob              | cron      |
| Kubernetes Job                  | job       |
| Namespace                       | ns        |
| NetworkPolicy                   | netp      |
| PersistentVolume                | pv        |
| PersistentVolumeClaim           | pvc       |
| Pod Template                    | pdt       |
| Role                            | role      |
| RoleBinding                     | rb        |
| Secret                          | sec       |
| Service                         | svc       |
| ServiceAccount                  | sa        |
| StatefulSet                     | ss        |
