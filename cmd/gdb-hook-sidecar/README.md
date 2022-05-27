# KubeVirt GDB hook sidecar

To use this hook, use following annotations:

```yaml
annotations:
  # Request the hook sidecar
  hooks.kubevirt.io/hookSidecars: '[{"image": "registry:5000/kubevirt/gdb-hook-sidecar:devel"}]'
  # Set GDBPort
  gdb.vm.kubevirt.io/GDBPort: 1235
```