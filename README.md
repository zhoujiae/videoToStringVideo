## 视频转字符画
#### 1.第一步我们通过 input[type="file"] 获取文件
#### 2.拿到文件之后，用 URL.createObjectURL来获取视频的路径
#### 3. 通过 ctx.drawImage 我们可以把某个 video 当前的图像渲染到 canvas里面
#### 4. ctx.getImageData 可以获取当前canvas 里面图片的色值，利用公式计算出灰度
#### 5. 根据灰度的深浅去匹配要显示的字符，深色匹配比较密集的字符，然后用 ctx.fillText重绘进去
