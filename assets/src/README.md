banner.png 的源。重建：

    chrome --headless --no-proxy-server --hide-scrollbars --force-device-scale-factor=2 \
      --window-size=1280,320 --screenshot=../banner.png "file://$(pwd)/banner.html"

必须给 file:// 绝对路径并加 --no-proxy-server，否则会被当成 URL 走代理，渲出错误页而不报错。
