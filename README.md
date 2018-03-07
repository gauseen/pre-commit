#### pre-commit
用 git 钩子 检测代码的规范性（JavaScript Standard 规范）
#### 启动项目步骤
```
# 克隆代码
git clone https://github.com/gauseen/pre-commit.git

# 更改远程仓库 URL
git remote set-url origin url  # url 需要是你自己的 git 仓库地址

# 下载项目依赖资源
npm install

# 更改 src 目录下的 test.js 文件，在 var faker = 'hello world !' 后面加个 ; （分号）

# 提交代码到 git 仓库
git add . && git commit -m "代码规范验证"


# 无法提交，因为代码不规范，报错信息如下

2:19  error  Extra semicolon # 意思就是不让加分号

# 删除分号后，再次提交，通过验证，成功提交。
```
