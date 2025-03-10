---
title: tiup cluster prune
summary: tiup cluster prune 命令用于在缩容集群时清理数据。对于某些组件，需要等数据调度完成后，用户手动执行该命令。选项包括 -h 或 --help，用于输出帮助信息。清理过程会生成日志。
---

# tiup cluster prune

在[缩容集群](/tiup/tiup-component-cluster-scale-in.md)时，对于某些组件，并不会立即停止服务并删除数据，而是需要等数据调度完成之后，用户手动执行 `tiup cluster prune` 命令清理。

## 语法

```shell
tiup cluster prune <cluster-name> [flags]
```

## 选项

### -h, --help

- 输出帮助信息。
- 数据类型：`BOOLEAN`
- 该选项默认关闭，默认值为 `false`。在命令中添加该选项，并传入 `true` 值或不传值，均可开启此功能。

## 输出

清理过程的日志。
