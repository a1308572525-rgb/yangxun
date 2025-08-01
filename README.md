# 我的个人网站

这是一个现代化的响应式个人网站，任何人都可以通过网址访问。

## 文件结构

```
├── index.html      # 主页面
├── styles.css      # 样式文件
├── script.js       # JavaScript交互
└── README.md       # 说明文档
```

## 本地预览

1. 双击 `index.html` 文件在浏览器中打开
2. 或者使用本地服务器：
   ```bash
   # 使用Python
   python -m http.server 8000
   
   # 使用Node.js
   npx serve .
   ```

## 部署到公网的步骤

### 方法一：使用GitHub Pages（免费）

1. **创建GitHub账号**（如果还没有）
2. **创建新仓库**：
   - 登录GitHub
   - 点击"New repository"
   - 仓库名填写：`your-username.github.io`
   - 选择Public
   - 点击"Create repository"

3. **上传文件**：
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/your-username/your-username.github.io.git
   git push -u origin main
   ```

4. **启用GitHub Pages**：
   - 进入仓库设置（Settings）
   - 找到"Pages"选项
   - Source选择"Deploy from a branch"
   - Branch选择"main"
   - 点击"Save"

5. **访问网站**：
   - 等待几分钟后，访问 `https://your-username.github.io`

### 方法二：使用Netlify（免费）

1. **注册Netlify账号**
2. **拖拽部署**：
   - 登录Netlify
   - 直接将网站文件夹拖拽到部署区域
   - 自动生成网址

3. **自定义域名**（可选）：
   - 在Netlify设置中添加自定义域名

### 方法三：使用Vercel（免费）

1. **注册Vercel账号**
2. **导入项目**：
   - 连接GitHub仓库
   - 或直接上传文件
3. **自动部署**：
   - Vercel会自动部署并生成网址

### 方法四：购买虚拟主机

1. **购买域名**（如阿里云、腾讯云）
2. **购买虚拟主机**或云服务器
3. **上传文件**：
   - 使用FTP工具上传网站文件
   - 或使用控制面板的文件管理器

## 推荐方案

对于初学者，我推荐使用 **GitHub Pages**，因为：
- 完全免费
- 操作简单
- 支持自定义域名
- 自动HTTPS
- 版本控制

## 自定义内容

修改以下文件来自定义你的网站：

- `index.html` - 修改文字内容
- `styles.css` - 修改颜色、字体、布局
- `script.js` - 添加更多交互功能

## 注意事项

1. 确保所有文件都在同一目录下
2. 文件名要区分大小写
3. 图片文件建议使用相对路径
4. 定期备份你的网站文件

## 技术支持

如果遇到问题，可以：
1. 检查浏览器控制台是否有错误
2. 确认文件路径是否正确
3. 查看GitHub Pages的部署日志 