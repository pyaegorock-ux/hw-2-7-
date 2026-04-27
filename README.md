# hw-2-7-
<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <title>HW23 - 艾菲爾鐵塔練習</title>
    <style>
        body { font-family: sans-serif; text-align: center; background: #f6f6f6; padding: 40px; }
        
        .gallery {
            display: flex;
            justify-content: space-around;
            align-items: center;
            margin-top: 30px;
        }

        /* 共用圖片基礎樣式 */
        img { border: 1px solid #ddd; background: white; padding: 5px; }

        /* 左圖：圓角 + 不變形 (PDF 提到的 cover) */
        .left {
            width: 300px;
            height: 300px;
            border-radius: 18px;
            object-fit: cover; 
        }

        /* 中圖：正圓形地球 */
        .center {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
        }

        /* 右圖：寬度33% + 高度300px + 形變 (PDF 提到的 fill) */
        .right {
            width: 33%;
            height: 300px;
            object-fit: fill; /* 這會產生 PDF 截圖中的擠壓感 */
        }

        .desc { font-size: 13px; color: #666; margin-top: 8px; }
    </style>
</head>
<body>

    <h2>CSS Object-fit & Radius Practice</h2>

    <div class="gallery">
        <div>
            <img src="https://images.unsplash.com/photo-1511739001486-6bfe10ce785f?w=400" class="left">
            <p class="desc">Radius 18px / object-fit: cover</p>
        </div>

        <div>
            <img src="https://images.unsplash.com/photo-1614730321146-b6fa6a46bcb4?w=300" class="center">
            <p class="desc">Circle Earth</p>
        </div>

        <div>
            <img src="https://images.unsplash.com/photo-1511739001486-6bfe10ce785f?w=400" class="right">
            <p class="desc">33% Width / object-fit: fill</p>
        </div>
    </div>

</body>
</html>


