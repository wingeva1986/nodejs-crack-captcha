# nodejs-crack-capcha
网易大航海之路内嵌滑动验证码识别，和叉叉助手配合使用，因为叉叉助手被封，项目已经用不了，但是后台识别代码还是有一定参考价值的，主要是opencv4nodejs的用法，先把验证码图片高斯模糊一下，然后canny边缘检测，然后再用jimp对处理后的图片做个扫描，扫描算法也很简单，就是找右下方的直角进行比对，最后返回滑动后的块x轴像素坐标，主要逻辑都在hackService.js里面。
这个是用nodejs+express做的后端，前端lua从手机上截图上传验证码图片，获得x轴坐标，再模拟滑动，前端的代码在另一个项目里面，还有游戏外挂逻辑的代码也在。

留个纪念~
