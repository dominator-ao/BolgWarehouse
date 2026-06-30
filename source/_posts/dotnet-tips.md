---
title: .NET 开发常用技巧
date: 2026-06-28 10:00:00
categories:
  - 技术
  - 后端
tags:
  - dotnet
  - csharp
  - sqlsugar
---

## 依赖注入

```csharp
// 注册服务
services.AddScoped<IMyService, MyService>();

// 构造函数注入
public class MyController : Controller
{
    private readonly IMyService _service;
    public MyController(IMyService service)
    {
        _service = service;
    }
}
```

## SqlSugar 常用操作

```csharp
// 查询
var list = await db.Queryable<Order>()
    .Where(x => x.Status == 1)
    .OrderByDescending(x => x.CreateTime)
    .ToListAsync();

// 分页
var page = await db.Queryable<Order>()
    .ToPageIndexListAsync(pageIndex, pageSize);
```

## 异步编程

```csharp
// 避免 async void
public async Task DoSomethingAsync()
{
    await Task.Delay(1000);
    Console.WriteLine("Done");
}
```

## 配置管理

```csharp
// 读取配置
var value = configuration["Section:Key"];

// 强类型绑定
services.Configure<AppSettings>(
    configuration.GetSection("AppSettings"));
```
