# DockerとViteを使用した環境構築

# 前提条件
- Docker Desktopをインストールしていること

# 環境構築方法
```
./shell.sh [サービス名]

ex) ./shell.sh node
```

# package.jsonの変更
プロジェクト内に配置しているpackage.jsonの「scripts - dev」の「vite」に「--host」を追加し、「vite --host」に変更してください。
```
{
	"name": "test",
	"private": true,
	"version": "0.0.0",
	"scripts": {
		"dev": "vite --host",
		"build": "vite build",
		"preview": "vite preview"
	},
	・・・
}
```

# 起動方法
```
cd vite-project
docker-compose up
```

# 停止方法
```
docker-compose down
```
