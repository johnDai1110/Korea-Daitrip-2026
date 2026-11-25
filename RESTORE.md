# 還原上一版楓葉網站

上一版提交：`4cb2a78e48a97608a0e49cacb67f46ecf26c96cf`

備份分支：`backup/maple-v1-before-redesign`

舊版預覽：https://johnDai1110.github.io/Korea-Daitrip-2026/previous/

如需恢復，可請 Codex「將釜山網站恢復為 backup/maple-v1-before-redesign 版本並重新部署」。會新增還原提交，保留歷史。

自行操作：

```powershell
git fetch origin
git switch main
git pull --ff-only origin main
git restore --source origin/backup/maple-v1-before-redesign -- index.html style.css app.js assets/busan-maple.webp .nojekyll
git add index.html style.css app.js assets/busan-maple.webp .nojekyll
git commit -m "Restore maple website v1"
git push origin main
```

GitHub Pages 會沿用既有設定重新部署。previous/ 保存原 HTML、CSS、JavaScript 與圖片，可獨立瀏覽。行李勾選沿用相同瀏覽器儲存鍵。
