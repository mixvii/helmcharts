# Sqlserver Helm Charts

## helm chart 仓库地址：

[helm-chart | helmcharts](https://mixvii.github.io/helmcharts)

## 使用方式：

### 1.添加helm仓库

> helm repo add masastack https://mixvii.github.io/helmcharts

### 2. 检查添加是否成功并更新包

> helm repo list 

```
> helm repo list
NAME            URL
...
masastack       https://mixvii.github.io/helmcharts
```

> helm repo update masastack

```
>helm repo update masastack
Hang tight while we grab the latest from your chart repositories...
...Successfully got an update from the "masastack" chart repository
Update Complete. ⎈Happy Helming!⎈
```

### 3. 查找需要安装的包

> helm search repo masastack 

```
>helm search repo masastack
NAME                    CHART VERSION   APP VERSION     DESCRIPTION
masastack/sqlserver     0.1.1           0.0.1           A Helm chart for Kubernetes
```

### 4. 选择需要的版本进行安装

> helm install sqlserver-dev masastack/sqlserver --version 0.1.1 
