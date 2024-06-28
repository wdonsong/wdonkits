---
title: "如何在大陆访问Vercel部署的项目"
date: 2024-06-28T19:43:31+08:00
draft: false
tags: []
showToc: true
TocOpen: false
hidemeta: false
comments: false
# canonicalURL: "https://canonical.url/to/page"
disableShare: true
disableHLJS: false
hideSummary: true
searchHidden: false
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: true
ShowRssButtonInSectionTermList: true
UseHugoToc: true
cover:
  image: "<image path/url>" # image path/url
  alt: "<alt text>" # alt text
  caption: "<text>" # display caption under cover
  relative: false # when using page bundles set this to true
  hidden: true # only hide on current single page
---

## 在 Vercel 部署项目

在 Vercel 部署自己的项目，在 Vercel 授权 github 账号以后，可以很方便地一键部署项目，在更新代码以后会自动进行重新部署很方便。

### 买一个域名

在阿里云，腾讯云等域名服务商购买一个域名，.xyz 之类的域名很便宜。

### 在 Cloudflare 添加站点

注册 Cloudflare 账号，然后把购买的域名添加进去，会得到 Cloudflare 的名称服务器的地址，然后去域名服务商的域名解析设置中把名称服务器的地址设置为 Cloudflare 的。

### 在 Vercel 设置自定义域名

在 Vercel 中给项目设置好想要的域名，然后在 Cloudflare 中设置添加 DNS 的 CNAME 记录，把这个域名指向 Vercel 的服务器。
